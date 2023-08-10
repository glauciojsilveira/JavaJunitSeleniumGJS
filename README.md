## Java-Junit-Selenium
[![Travis Status](https://travis-ci.org/saucelabs-sample-test-frameworks/Java-Junit-Selenium.svg?branch=master)](https://travis-ci.org/saucelabs-sample-test-frameworks/Java-Junit-Selenium)

Este código é fornecido "COMO ESTÁ" sem garantia de qualquer tipo, expressa ou implícita, incluindo, sem limitação, quaisquer garantias implícitas de condição, uso ininterrupto, comercialização, adequação a uma finalidade específica ou não violação. Seus testes e ambientes de teste podem exigir que você modifique esta estrutura. Problemas relacionados a esta estrutura devem ser enviados por meio do GitHub. Para questões relacionadas à integração do Sauce Labs, consulte a documentação do Sauce Labs em https://wiki.saucelabs.com/. Esta estrutura não é mantido pelo suporte da Sauce Labs
### Environment Setup

1. Global Dependencies
    * Install [Maven](https://maven.apache.org/install.html)
    * Or Install Maven with [Homebrew](http://brew.sh/) (Easier)
    ```
    $ brew install maven
    ```
2. Sauce Labs Credentials
    * In the terminal, export your Sauce Labs credentials as environmental variables:
    ```
    $ export SAUCE_USERNAME=<your Sauce Labs username>
    $ export SAUCE_ACCESS_KEY=<your Sauce Labs access key>
    ```
3. Project Dependencies
    * Check that packages are available
    ```
    $ cd Java-Junit-Selenium
    $ mvn test-compile
    ```
    * Você também pode executar o comando abaixo para verificar se há dependências desatualizadas. Certifique-se de verificar e revisar as atualizações antes de editar seu arquivo pom.xml, pois elas podem não ser compatíveis com seu código.

    ```
    $ mvn versions:display-dependency-updates
    ```
    
### Running Tests

#####Testing in Parallel:
```
$ mvn test
```
[Sauce Labs Dashboard](https://saucelabs.com/beta/dashboard/)

### Advice/Troubleshooting
1.Pode ser útil usar um Java IDE como IntelliJ ou Eclipse para ajudar a solucionar possíveis problemas.
2.Pode haver latência adicional ao usar um webdriver remoto para executar testes no Sauce Labs. Timeouts and/or waits pode precisar ser aumentado.
    * [Selenium tips regarding explicit waits](https://wiki.saucelabs.com/display/DOCS/Best+Practice%3A+Use+Explicit+Waits)

### Resources
##### [Sauce Labs Documentation](https://wiki.saucelabs.com/)

##### [SeleniumHQ Documentation](http://www.seleniumhq.org/docs/)

##### [Junit Documentation](http://junit.org/javadoc/latest/index.html)

##### [Java Documentation](https://docs.oracle.com/javase/7/docs/api/)

##### [Stack Overflow](http://stackoverflow.com/)
*Um ótimo recurso para procurar problemas não cobertos explicitamente pela documentação.


