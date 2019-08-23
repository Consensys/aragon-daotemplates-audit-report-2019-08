```
$ solium --version
Solium version 1.2.4
```

```console

shared/contracts/BaseTemplate.sol
  160:4    warning    Line exceeds the limit of 145 characters    max-len
  165:4    warning    Line exceeds the limit of 145 characters    max-len
  185:4    warning    Line exceeds the limit of 145 characters    max-len
  186:8    warning    Line exceeds the limit of 145 characters    max-len
  201:4    warning    Line exceeds the limit of 145 characters    max-len
  213:4    warning    Line exceeds the limit of 145 characters    max-len
  235:4    warning    Line exceeds the limit of 145 characters    max-len

shared/contracts/Migrations.sol
  4:2     error      Only use indent of 4 spaces.                   indentation
  5:2     error      Only use indent of 4 spaces.                   indentation
  7:2     error      Only use indent of 4 spaces.                   indentation
  9:0     error      Only use indent of 4 spaces.                   indentation
  11:2    error      Only use indent of 4 spaces.                   indentation
  11:2    warning    Constructor declaration style is deprecated    constructor
  13:0    error      Only use indent of 4 spaces.                   indentation
  15:2    error      Only use indent of 4 spaces.                   indentation
  17:0    error      Only use indent of 4 spaces.                   indentation
  19:2    error      Only use indent of 4 spaces.                   indentation
  22:0    error      Only use indent of 4 spaces.                   indentation

shared/contracts/test/mocks/ExecutionTarget.sol
  13:8    warning    Provide an error message for revert().    error-reason

shared/contracts/test/mocks/Timestamp.sol
  6:15    warning    Avoid using 'now' (alias to 'block.timestamp').    security/no-block-members

templates/trust/contracts/TrustTemplate.sol
  206:9    error    Only use indent of 8 spaces.    indentation
  207:9    error    Only use indent of 8 spaces.    indentation
  208:9    error    Only use indent of 8 spaces.    indentation
  209:9    error    Only use indent of 8 spaces.    indentation

✖ 14 errors, 10 warnings found.
```

## Solhint

```$ solhint --version
2.0.0-alpha.3
```

```console

shared/contracts/BaseTemplate.sol
   62:2  error  Line length must be no more than 120 but current length is 128  max-line-length
   87:2  error  Line length must be no more than 120 but current length is 133  max-line-length
  116:2  error  Line length must be no more than 120 but current length is 131  max-line-length
  156:2  error  Line length must be no more than 120 but current length is 125  max-line-length
  160:2  error  Line length must be no more than 120 but current length is 146  max-line-length
  161:2  error  Line length must be no more than 120 but current length is 134  max-line-length
  165:2  error  Line length must be no more than 120 but current length is 147  max-line-length
  173:2  error  Line length must be no more than 120 but current length is 140  max-line-length
  174:2  error  Line length must be no more than 120 but current length is 135  max-line-length
  185:2  error  Line length must be no more than 120 but current length is 161  max-line-length
  186:2  error  Line length must be no more than 120 but current length is 152  max-line-length
  201:2  error  Line length must be no more than 120 but current length is 158  max-line-length
  213:2  error  Line length must be no more than 120 but current length is 188  max-line-length
  235:2  error  Line length must be no more than 120 but current length is 150  max-line-length
  242:2  error  Line length must be no more than 120 but current length is 128  max-line-length
  247:2  error  Line length must be no more than 120 but current length is 126  max-line-length
  283:2  error  Line length must be no more than 120 but current length is 122  max-line-length
  295:2  error  Line length must be no more than 120 but current length is 130  max-line-length

shared/contracts/Migrations.sol
   4:3  error  Expected indentation of 4 spaces but found 2  indent
   5:3  error  Expected indentation of 4 spaces but found 2  indent
   7:3  error  Expected indentation of 4 spaces but found 2  indent
   8:5  error  Expected indentation of 8 spaces but found 4  indent
   9:3  error  Expected indentation of 4 spaces but found 2  indent
  11:3  error  Expected indentation of 4 spaces but found 2  indent
  12:5  error  Expected indentation of 8 spaces but found 4  indent
  13:3  error  Expected indentation of 4 spaces but found 2  indent
  15:3  error  Expected indentation of 4 spaces but found 2  indent
  16:5  error  Expected indentation of 8 spaces but found 4  indent
  17:3  error  Expected indentation of 4 spaces but found 2  indent
  19:3  error  Expected indentation of 4 spaces but found 2  indent
  20:5  error  Expected indentation of 8 spaces but found 4  indent
  21:5  error  Expected indentation of 8 spaces but found 4  indent
  22:3  error  Expected indentation of 4 spaces but found 2  indent

templates/bare/contracts/BareTemplate.sol
  19:2  error  Line length must be no more than 120 but current length is 136  max-line-length

templates/company-board/contracts/CompanyBoardTemplate.sol
   48:2  error  Line length must be no more than 120 but current length is 146  max-line-length
   49:2  error  Line length must be no more than 120 but current length is 146  max-line-length
   78:2  error  Line length must be no more than 120 but current length is 122  max-line-length
   80:2  error  Line length must be no more than 120 but current length is 130  max-line-length
  108:2  error  Line length must be no more than 120 but current length is 122  max-line-length
  110:2  error  Line length must be no more than 120 but current length is 130  max-line-length
  112:2  error  Line length must be no more than 120 but current length is 132  max-line-length
  113:2  error  Line length must be no more than 120 but current length is 137  max-line-length
  152:2  error  Line length must be no more than 120 but current length is 126  max-line-length
  153:2  error  Line length must be no more than 120 but current length is 126  max-line-length
  181:2  error  Line length must be no more than 120 but current length is 128  max-line-length
  194:2  error  Line length must be no more than 120 but current length is 128  max-line-length
  195:2  error  Line length must be no more than 120 but current length is 144  max-line-length
  212:2  error  Line length must be no more than 120 but current length is 125  max-line-length

templates/company/contracts/CompanyTemplate.sol
   34:2  error  Line length must be no more than 120 but current length is 135  max-line-length
   35:2  error  Line length must be no more than 120 but current length is 130  max-line-length
   70:2  error  Line length must be no more than 120 but current length is 135  max-line-length
   71:2  error  Line length must be no more than 120 but current length is 130  max-line-length
   97:2  error  Line length must be no more than 120 but current length is 135  max-line-length
   98:2  error  Line length must be no more than 120 but current length is 130  max-line-length
  100:2  error  Line length must be no more than 120 but current length is 132  max-line-length
  101:2  error  Line length must be no more than 120 but current length is 131  max-line-length
  117:2  error  Line length must be no more than 120 but current length is 134  max-line-length
  137:2  error  Line length must be no more than 120 but current length is 128  max-line-length
  147:2  error  Line length must be no more than 120 but current length is 133  max-line-length
  148:2  error  Line length must be no more than 120 but current length is 144  max-line-length
  188:2  error  Line length must be no more than 120 but current length is 137  max-line-length

templates/membership/contracts/MembershipTemplate.sol
   32:2  error  Line length must be no more than 120 but current length is 135  max-line-length
   33:2  error  Line length must be no more than 120 but current length is 130  max-line-length
   66:2  error  Line length must be no more than 120 but current length is 135  max-line-length
   67:2  error  Line length must be no more than 120 but current length is 130  max-line-length
   78:2  error  Indentation is incorrect                                        indent
   91:2  error  Line length must be no more than 120 but current length is 135  max-line-length
   92:2  error  Line length must be no more than 120 but current length is 130  max-line-length
   94:2  error  Line length must be no more than 120 but current length is 132  max-line-length
   95:2  error  Line length must be no more than 120 but current length is 131  max-line-length
  110:2  error  Line length must be no more than 120 but current length is 125  max-line-length
  129:2  error  Line length must be no more than 120 but current length is 128  max-line-length
  139:2  error  Line length must be no more than 120 but current length is 133  max-line-length
  140:2  error  Line length must be no more than 120 but current length is 144  max-line-length

templates/reputation/contracts/ReputationTemplate.sol
   34:2  error  Line length must be no more than 120 but current length is 135  max-line-length
   35:2  error  Line length must be no more than 120 but current length is 130  max-line-length
   70:2  error  Line length must be no more than 120 but current length is 135  max-line-length
   71:2  error  Line length must be no more than 120 but current length is 130  max-line-length
   97:2  error  Line length must be no more than 120 but current length is 135  max-line-length
   98:2  error  Line length must be no more than 120 but current length is 130  max-line-length
  100:2  error  Line length must be no more than 120 but current length is 132  max-line-length
  101:2  error  Line length must be no more than 120 but current length is 131  max-line-length
  117:2  error  Line length must be no more than 120 but current length is 134  max-line-length
  137:2  error  Line length must be no more than 120 but current length is 128  max-line-length
  147:2  error  Line length must be no more than 120 but current length is 133  max-line-length
  148:2  error  Line length must be no more than 120 but current length is 144  max-line-length
  188:2  error  Line length must be no more than 120 but current length is 140  max-line-length

templates/trust/contracts/MultiSigWallet.sol
  248:2   error  Line length must be no more than 120 but current length is 128  max-line-length
  301:13  error  Expected indentation of 8 spaces but found 12                   indent

templates/trust/contracts/TrustTemplate.sol
   31:2   error  Line length must be no more than 120 but current length is 124  max-line-length
  132:2   error  Line length must be no more than 120 but current length is 137  max-line-length
  155:2   error  Line length must be no more than 120 but current length is 132  max-line-length
  177:2   error  Line length must be no more than 120 but current length is 127  max-line-length
  178:2   error  Line length must be no more than 120 but current length is 132  max-line-length
  179:2   error  Line length must be no more than 120 but current length is 121  max-line-length
  180:2   error  Line length must be no more than 120 but current length is 125  max-line-length
  203:2   error  Line length must be no more than 120 but current length is 140  max-line-length
  206:10  error  Expected indentation of 8 spaces but found 9                    indent
  207:10  error  Expected indentation of 8 spaces but found 9                    indent
  208:10  error  Expected indentation of 8 spaces but found 9                    indent
  209:10  error  Expected indentation of 8 spaces but found 9                    indent
  216:2   error  Line length must be no more than 120 but current length is 143  max-line-length
  239:2   error  Line length must be no more than 120 but current length is 140  max-line-length

✖ 103 problems (103 errors, 0 warnings)
```