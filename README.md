### Github Actions Examples and Notes

```yml
name: Building Blocks

on: push

jobs:
    echo-hello:
        runs-on: ubuntu-latest
        steps:
            - name: Say hello
              run: echo "Hello World!"
    echo-goodbye:
        runs-on: ubuntu-latest
        steps:
            - name: Failed step
              run: |
                  echo "This will fail"
                  exit 0
            - name: Say goodbye
              run: echo "Goodbye!"
```
