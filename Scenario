Feature: User Registration

  Scenario: Register a user with valid data
    Given user has registration data
    When user sends a registration request
    Then the response status code should be 200
    And the response should contain a token

  Scenario: Register a user with missing data
    Given user has incomplete registration data
    When user sends a registration request
    Then the response status code should be 400
    And the response should contain an error message



=================================================================================================================

Feature: User Login

  Scenario: Login with valid credentials
    Given user has valid login data
    When user sends a login request
    Then the response status code should be 200
    And the response should contain a token
    And the response time should be within acceptable range
    And the response content type should be application/json

  Scenario: Login with invalid credentials
    Given user has invalid login data
    When user sends a login request
    Then the response status code should be 400
    And the response should contain an error message
