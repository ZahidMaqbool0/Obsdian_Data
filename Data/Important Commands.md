# Maestro Studio

### Run automatic maestro studio code using terminal
Run the maestro test using Terminal 
```maestro
maestro test maestrofoldername/filename.yaml
```

### Report Generated in Simple Text format
Report Generate in text format use this command.
```maestro
maestro test maestrofoldername/filename.yaml > maestro-report.txt
```

### XML report convert into Excel file
if we generate the maestro studio report in excel format. then follow this step.

**Step 1:** Report generate in XML
if we define the test case in one file, like this. and bottom given testcase name is (we use the name we provide the every test case separately) 
```yaml
flows:
  - "testcases/**"

executionOrder:

  continueOnFailure: false

  flowsOrder:
    - launchAppFlow # testcase 1
    - auth_login_with_valid_credentials # testcase 2
    - home_display_feed_section # testcase 3
    - home_display_connect_section # testcase 4
    - menu_open_menu # testcase 5
    - mycampus_my_campus_secation # testcase 6
    - post create post_section # testcase 7
```

run project using this command. if follow top written structure.
```maestro
maestro test . --format junit --output reports/xml-report/xml-report.xml
```

if we run just one test case.. mean one file.. 
```mastro
maestro test maestro/master.yaml --format junit --output myReport.xml
```

**Step 2:** Run this bottom given command to install package to convert XML into Excel format (just one time simple install the one package i project)
```maestro
npm install xml2js xlsx --legacy-peer-deps
```

**Step 3:** Create one file in ***==JavaScript==*** format like. *(filename.js)* and in this file paste the bottom given code.
```javascript
const fs = require("fs");
const path = require("path");
const xml2js = require("xml2js");
const XLSX = require("xlsx");

/*
  📂 File Paths
*/

const xmlFile = path.join(__dirname, "../reports/xml-report/xml-report.xml");
const outputFile = path.join(__dirname, "../reports/excel-report/maestro-final-report.xlsx");

/*
  ❌ Check if XML Exists
*/

if (!fs.existsSync(xmlFile)) {
  console.log("❌ XML report not found. Run maestro test first.");
  process.exit(1);
}
  
const xmlData = fs.readFileSync(xmlFile, "utf-8");

 /*
  🔎 Extract Failure Reason Safely
*/

function extractFailureReason(failure) {

  if (!failure) return "Unknown Failure";
  if (typeof failure === "string") return failure.trim();
  if (failure._) return failure._.trim();
  if (failure.$ && failure.$.message)
    return failure.$.message.trim();
  return "Unknown Failure";
  
}
 
/*
  🧠 Parse XML
*/

xml2js.parseString(xmlData, (err, result) => {

  if (err) {
    console.log("❌ Error parsing XML:", err.message);
    return;
  }

  const testcases =
    result?.testsuites?.testsuite?.[0]?.testcase || [];
    
    if (testcases.length === 0) {
    console.log("⚠️ No testcases found in XML.");
    return;

  }

  /*
    ✅ Automatically process all flows
 */ 

  const rows = testcases.map((test, index) => {

    const rawName = test.$?.name || "";

    const fileName = rawName.replace(".yaml", "");

  

    const moduleName =

      fileName.split("_")[0]?.toUpperCase() || "GENERAL";

  

    const testName = fileName
      .split("_")
      .slice(1)
      .join(" ");

    const isFail = Array.isArray(test.failure);
    let remark = "OK";

    if (isFail) {
      remark = extractFailureReason(test.failure[0]);
    }
 
    return {
      Order: index + 1,
      Module: moduleName,
      Test_Name: testName || fileName,
      File_Name: rawName,
      Status: isFail ? "FAILED ❌" : "PASSED ✅",
      Time_Seconds: test.$?.time || "0",
      Remark: remark
    };

  });

  /*
    📊 Create Excel
  */

  const worksheet = XLSX.utils.json_to_sheet(rows);
  const workbook = XLSX.utils.book_new();

  XLSX.utils.book_append_sheet(workbook, worksheet, "Execution Flow");
  XLSX.writeFile(workbook, outputFile);
  console.log("🎉 Excel Report Generated Successfully!");

});
```


**Step 4:** Run this command and in this command use file we create in step ***==Step 3==*** 
```maestro
node filename.js
```

**Step 5:** One report automatic generate in project like (filename.xlsx)

# Scrcpy Command (Show VSCODE Physical Mobile Device)
Scrcpy like a tool, it is show the mobile device on desktop screen. mean physical device show on window screen. 
=> Run this command to scrcpy is always on top no minimize.
```bash
scrcpy --always-on-top --stay-awake
```




zjvizjvzj
lmcmzm
vkxdnn

