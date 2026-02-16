# WebMCP Tests

This directory contains test cases for the WebMCP specification.

## Test Structure

Tests follow the [Web Platform Tests](https://web-platform-tests.org/) conventions and use the testharness.js framework.

### Running Tests

Tests can be run in a browser that implements the WebMCP API. The tests verify:

- Interface availability and basic API surface
- Tool registration and unregistration
- Schema validation
- SecureContext requirements
- Error handling

## Test Files

- `model-context/` - Tests for the ModelContext interface and related functionality
  - `model-context-interface.html` - Basic interface availability tests
  - `register-tool-basic.html` - Tool registration tests
  - `unregister-tool-basic.html` - Tool unregistration tests
  - `context-methods.html` - Context method tests (provideContext, clearContext)
  - `secure-context.html` - SecureContext requirement tests
  - `schema-validation.html` - Tool input schema validation tests

## Contributing

When adding new tests, ensure they:
1. Use testharness.js framework
2. Include proper test metadata (title, assert messages)
3. Test both success and failure cases
4. Include clear documentation of what is being tested
