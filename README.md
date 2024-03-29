# Sample Spring Boot app to check the behavior of OWASP Dependency Check

See [the doc](https://jeremylong.github.io/DependencyCheck/index.html) for OWASP Dependency Check tool.
This app just installs the Gradle plugin of OWASP Dependency Check tool into the sample Spring Boot app generated by [Spring Initializr](https://start.spring.io/).

# How to use this sample

1. Clone this repo

    ```
    git clone https://github.com/lethe2211/owasp-dependencycheck-sample.git
    ```

2. Run the dependency check

    ```
    cd owasp-dependencycheck-sample

    ## Mac / Linux
    ./gradlew clean dependencyCheckAnalyze

    ## Windows
    gradlew.bat clean dependencyCheckAnalyze
    ```
   
3. Check the generated report

    ```
    # Open the generated `build/reports/dependency-check-report.html` in your browser

    ## Mac
    open build/reports/dependency-check-report.html
    ```

    ![image](https://user-images.githubusercontent.com/1718146/193516222-8041542a-9ecb-4e99-881a-f9b738cf50c7.png)

4. You can play by modifying some config in build.gradle or installing a vulnerable software
