# jmeter-selenium-browserstack

In this project you can capture page load time of your web app using Jmeter, Selenium and BrowserStack.

[BrowserStack](https://www.browserstack.com) is a great tool for cross browser testing. Using BrowserStack you can execute your test in Chrome, Firefox and IE


# PreRequisite
- Knowledge of Jmeter (beginner can execute this)
- Jmeter latest stable version (I am using 5.4.1)
- Java 8 or higher
- [Jmeter Webdriver Plugin](https://jmeter-plugins.org/?search=jpgc-webdriver)
- BrowserStack Licence

## Execution

- Clone the repo and open it in your local Jmeter
- Open jp@gc - Remote Driver Config under Thread Group
- Add Selenium Grip URL as "https://username:accesskey@hub-cloud.browserstack.com/wd/hub"
- Select the preferred browser
- Run the test

## Reporting

You can generate the html report in your local as well using below command
`sh jmeter -n -t <path_to_your_jmx_file>/sample.jmx -l  <path_to_your_jmx_file>/<uniqueName>.csv -e -o <path_to_your_jmx_file>/<uniqueName>`
