### CODE ORGANISATION


    ── app/ 
    ├── build/
    ├── docs/
    ├── src/
    │   └── secur3dit/
    │       ├── filters/
    │       │   ├── Filters.java
    |       |   ├── Kernels.java
    │       │   └── Helpers.java
    │       ├── crypto/
    │       │   ├── AES256CTR.java
    │       │   ├── AES256.java
    │       │   ├── Constants.java
    │       │   └── Helpers.java
    │       ├── ui/
    |       |   |── images/
            |   ├── UifxmlController.java
    │       │   ├── design.css
    │       │   ├── encryption.fxml
    │       │   ├── encryptionController.java
    │       │   ├── filterDesign.css
    │       │   ├── homepage.fxml
    │       │   ├── homepageController.java
    │       │   └── uifxml.fxml
    │       └── Main.java
    ├── tests/
    |    ├── TEST_DATA.csv
    |    └── TestAES256.java
    ├── LICENSE.md
    └── README.md
