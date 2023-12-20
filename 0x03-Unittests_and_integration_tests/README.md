# Unittests and Integration Tests

This project involves tasks related to writing unittests and integration tests in Python 3.

## Tasks Overview

### 0. Parameterize a unit test

**File:** [test_utils.py](test_utils.py)

In this task, the `TestAccessNestedMap` class is created to test the `utils.access_nested_map` function. The `test_access_nested_map` method is implemented to test the function with different inputs using `@parameterized.expand`. It checks whether the function returns the expected result for each input.

### 1. Parameterize a unit test

**File:** [test_utils.py](test_utils.py)

The `TestAccessNestedMap` class is extended to include the `test_access_nested_map_exception` method. This method uses `assertRaises` to test that a `KeyError` is raised for specific inputs. The exception message is also checked to ensure it matches the expected value.

### 2. Mock HTTP calls

**File:** [test_utils.py](test_utils.py)

The `TestGetJson` class is introduced to test the `utils.get_json` function. The `test_get_json` method uses `@patch` to mock `requests.get` and ensure it returns a `Mock` object with a `json` method. The function is then tested for different inputs, and it is verified that the mocked `get` method is called exactly once with the correct arguments.

### 3. Parameterize and patch

**File:** [test_utils.py](test_utils.py)

The `TestMemoize` class is created to test the `utils.memoize` decorator. The `test_memoize` method defines a class (`TestClass`) with a method (`a_method`) and a memoized property (`a_property`). It uses `@patch` to mock `a_method` and ensures that calling `a_property` twice returns the correct result, and `a_method` is only called once.

### 4. Parameterize and patch as decorators

**File:** [test_client.py](test_client.py)

The `TestGithubOrgClient` class is introduced to test the `client.GithubOrgClient` class. The `test_org` method uses `@patch` as a decorator to mock `get_json` and ensure it is called once with the correct arguments. It is also parametrized with different `org` examples.

### 5. Mocking a property

**File:** [test_client.py](test_client.py)

The `TestGithubOrgClient` class is extended with the `test_public_repos_url` method. This method tests the `GithubOrgClient._public_repos_url` property using `@patch` to mock `GithubOrgClient.org` and return a known payload. It checks whether the result of `_public_repos_url` is as expected based on the mocked payload.

### 6. More patching

**File:** [test_client.py](test_client.py)

The `TestGithubOrgClient` class is further extended with the `test_public_repos` method. This method tests the `GithubOrgClient.public_repos` method using `@patch` to mock `get_json` and ensure it returns a payload of choice. It also patches `GithubOrgClient._public_repos_url` to return a value of choice. The test verifies that the list of repos is as expected and that the mocked property and `get_json` are called once.

### 7. Parameterize

**File:** [test_client.py](test_client.py)

The `TestGithubOrgClient` class is extended with the `test_has_license` method. This method uses `@parameterized.expand` to parametrize the test with different inputs and expected returned values. It checks whether the `GithubOrgClient.has_license` method behaves as expected.

### 8. Integration test: fixtures

**File:** [test_client.py](test_client.py)

The `TestIntegrationGithubOrgClient` class is created for integration testing. It uses `@parameterized_class` to parametrize the class with fixtures from [fixtures.py](fixtures.py). The `setUpClass` and `tearDownClass` methods are implemented to mock `requests.get` and create a patcher for `get_json`. The test checks whether the `GithubOrgClient.public_repos` method returns the expected results based on the fixtures.

### 9. Integration tests

**File:** [test_client.py](test_client.py)

The `TestIntegrationGithubOrgClient` class is further extended with the `test_public_repos` and `test_public_repos_with_license` methods. These methods test the `GithubOrgClient.public_repos` method with different arguments and check whether the results match the expected values based on the fixtures.

## Resources

- [unittest — Unit testing framework](https://intranet.alxswe.com/rltoken/a_AEObGK8jeqPtTPmm-gIA)
- [unittest.mock — mock object library](https://intranet.alxswe.com/rltoken/PKetnACd7FfRiU8_kpe5EA)
- [How to mock a readonly property with mock?](https://intranet.alxswe.com/rltoken/2ueVPK1kWZuz525FvZ1v2Q)
- [parameterized](https://intranet.alxswe.com/rltoken/mI7qc3Y42aZ7GTlLXDxgEg)
- [Memoization](https://intranet.alxswe.com/rltoken/x83Hdr54q4Vax5xQ2Z3HSA)