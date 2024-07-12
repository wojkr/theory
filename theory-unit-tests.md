### MOCKS

> Right call, Right Numbers of calls with right parameters

- replaces external intefaces
- checks:
  - is the function called or not,
  - how many times fction was called.
  - what parameters are passed when called

### STUBS

> generates predefined outputs

- Returns success/failure/exception,
- Chekcs the behaviour of code under test in case of these return values

### FAKES

> Almost working implementation (ex. http server, in memory DB)

- instead going to internet it connects to a local(limited implementation
- checks the behaviour with respect to the actual data it receives from the server
- created specifically for this test,
- How the code behaves when it really gets lots of data
