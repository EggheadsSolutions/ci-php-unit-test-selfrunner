# php-unit-test-selfrunner

##Пример запуска:   
```
    name: Unit Test

    on: [ pull_request ]

    jobs:
    UnitTest:
        runs-on: self-hosted
        steps:
        - uses: EggheadsSolutions/php-unit-test-selfrunner@v1
            with:
            app-local-php: "${{ secrets.APP_LOCAL_PHP_DEV }}"
            ca-pem: "${{ secrets.CA_PEM }}"
```