#  java-playwright-browserstack
This repo contains samples for running junit-5 playwright tests on Browserstack Turboscale.

## Setup
* Clone the repo `git clone git@github.com:BrowserStackCE/example-turboscale-java-playwrigt.git`
* Install dependencies `mvn install`
* Update credentials in the `grid.browserstack.yml` file with your [BrowserStack Username and Access Key](https://www.browserstack.com/accounts/settings).
* The `grid.browserstack.yml` file is already updated with the capability turboScale: true. If required specify the grid name in turboScaleOptions capability

## Running tests:
* To run a sample tests, run `mvn test -P ats-test`.


## Notes
* You can view your test results on the [BrowserStack Turboscale dashboard](https://grid.browserstack.com/dashboard/)
* You can also export the environment variables for the Username and Access Key of your BrowserStack account.

  * For Unix-like or Mac machines:
  ```
  export BROWSERSTACK_USERNAME=<browserstack-username> &&
  export BROWSERSTACK_ACCESS_KEY=<browserstack-access-key>
  ```
  
  * For Windows:
  ```
  set BROWSERSTACK_USERNAME=<browserstack-username>
  set BROWSERSTACK_ACCESS_KEY=<browserstack-access-key>
  ```
