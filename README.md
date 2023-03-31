# stk-cli-action

[![Action test Ubuntu](https://github.com/stack-spot/stk-cli-action/actions/workflows/action-test-ubuntu.yml/badge.svg)](https://github.com/stack-spot/stk-cli-action/actions/workflows/action-test-ubuntu.yml) [![Action test MacOS](https://github.com/stack-spot/stk-cli-action/actions/workflows/action-test-macos.yml/badge.svg)](https://github.com/stack-spot/stk-cli-action/actions/workflows/action-test-macos.yml) [![Action test Windows](https://github.com/stack-spot/stk-cli-action/actions/workflows/action-test-windows.yml/badge.svg)](https://github.com/stack-spot/stk-cli-action/actions/workflows/action-test-windows.yml)

GitHub action to install StackSpot CLI :octocat:

_**Note**: This action is supported on all runners operating systems (`ubuntu`, `macos`, `windows`)_

## 📚 Usage

### Requirements

To get the account keys (`CLIENT_ID`, `CLIENT_KEY` and `REALM`), please login using a **ADMIN** user on the [StackSpot Portal](https://stackspot.com), and generate new keys at [https://stackspot.com/en/settings/access-token](https://stackspot.com/en/settings/access-token).

### Use Case

```yaml
    steps:
      - uses: stack-spot/stk-cli-action@v1.1
        with:
          client_id: ${{ secrets.CLIENT_ID }}
          client_key: ${{ secrets.CLIENT_KEY }}
          realm: ${{ secrets.REALM }}

      - run: stk import stack <STACK_URL>
```

## License

[Apache License 2.0](https://github.com/stack-spot/stk-cli-action/blob/main/LICENSE)

