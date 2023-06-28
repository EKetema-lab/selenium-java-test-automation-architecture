# Selenium Java Test Automation Architecture

Ready-to-use UI Test Automation Architecture using Java and Selenium WebDriver. 

## Installation Steps

In order to use the framework:

1. [Fork](https://github.com/Tahanima/selenium-java-test-automation-architecture/fork) the repository.
2. Clone, i.e, download your copy of the repository to your local machine using
```
git clone https://github.com/[your_username]/selenium-java-test-automation-architecture.git
```
3. Import the project in [IntelliJ IDEA](https://www.jetbrains.com/idea/download/).
4. Make your desired changes.
5. Use IntelliJ IDEA to run your desired tests. Alternatively, you can use the terminal to run the tests, for example `./gradlew test -Dbrowser=firefox -Dheadless=false` to run all the tests using the firefox browser in headful mode.

## Languages and Frameworks

The project uses the following:

- *[Java 11](https://openjdk.java.net/projects/jdk/11/)* as the programming language.
- *[Selenium WebDriver](https://www.selenium.dev/)* as the web browser automation framework using the Java binding.
- *[WebDriverManager](https://bonigarcia.dev/webdrivermanager/)* as the browser driver management library.
- *[Univocity Parsers](https://www.univocity.com/pages/univocity_parsers_tutorial)* to parse and handle CSV files.
- *[TestNG](https://testng.org/doc/)* as the testing framework.
- *[AssertJ](https://assertj.github.io/doc/)* as the assertion library.
- *[Lombok](https://projectlombok.org/)* to generate getters.
- *[Owner](http://owner.aeonbits.org/)* to minimize the code to handle properties file.
- *[Extent Reports](https://www.extentreports.com/)* as the test reporting strategy.
- *[Selenium Shutterbug](https://github.com/assertthat/selenium-shutterbug)* for capturing screenshots.
- *[Gradle](https://gradle.org/)* as the Java build tool.
- *[IntelliJ IDEA](https://www.jetbrains.com/idea/)* as the IDE.

## Project Structure

The project is structured as follows:

```bash
📦 selenium-java-test-automation-architecture
├─ .github
│  ├─ FUNDING.yml
│  └─ workflows
│     └─ test-execution.yml
├─ .gitignore
├─ LICENSE
├─ README.md
├─ build.gradle
├─ gradle
│  └─ wrapper
│     ├─ gradle-wrapper.jar
│     └─ gradle-wrapper.properties
├─ gradlew
├─ gradlew.bat
├─ script
│  └─ install_chrome.sh
├─ settings.gradle
└─ src
   ├─ main
   │  └─ java
   │     └─ io
   │        └─ github
   │           └─ tahanima
   │              ├─ config
   │              │  ├─ Configuration.java
   │              │  └─ ConfigurationManager.java
   │              ├─ data
   │              │  ├─ BaseData.java
   │              │  ├─ LoginData.java
   │              │  └─ ProductsData.java
   │              ├─ factory
   │              │  ├─ BasePageFactory.java
   │              │  └─ BrowserFactory.java
   │              ├─ report
   │              │  └─ ExtentReportManager.java
   │              └─ ui
   │                 ├─ component
   │                 │  ├─ BaseComponent.java
   │                 │  ├─ Header.java
   │                 │  └─ SideNavMenu.java
   │                 └─ page
   │                    ├─ BasePage.java
   │                    ├─ LoginPage.java
   │                    └─ ProductsPage.java
   └─ test
      ├─ java
      │  └─ io
      │     └─ github
      │        └─ tahanima
      │           ├─ e2e
      │           │  ├─ BaseE2ETest.java
      │           │  ├─ LoginE2ETest.java
      │           │  └─ ProductsE2ETest.java
      │           └─ util
      │              ├─ DataProviderUtil.java
      │              ├─ TestListener.java
      │              └─ TestRetry.java
      └─ resources
         ├─ config.properties
         └─ testdata
            ├─ login.csv
            └─ products.csv
```
