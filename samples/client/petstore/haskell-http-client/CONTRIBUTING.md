### Rebuild jar

```
    (cd ../../../..; mvn package);
```

### Regenerate Template

1. Run the shell script `haskell-http-client-petstore.sh` to update the Petstore sample

```bash
    (cd ../../../..; ./bin/haskell-http-client-petstore.sh);
```

### Typecheck, Build and run Unit tests

2. Check that the following commands complete build without any errors

```bash
    (stack clean && stack haddock && stack test);
    (cd ./example-app; stack clean && stack build);
    (cd ./tests-integration; stack clean && stack build --no-run-tests);
```

### Integration Tests

3. run the integration tests as described in `./tests-integration/README.md`

