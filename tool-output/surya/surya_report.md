## Sūrya's Description Report

### Files Description Table


|  File Name  |  SHA-1 Hash  |
|-------------|--------------|
| shared/contracts/BaseTemplate.sol | a085e3acea08f4ba74f1f6afbbd00045d011db22 |
| shared/contracts/TokenCache.sol | e93cbe72cf6f804e436889f1fa4add21cd5bfe00 |
| templates/bare/contracts/BareTemplate.sol | 7f02ee0a1af3e8d9089a71eb782ef9d18e8aa017 |
| templates/company-board/contracts/CompanyBoardTemplate.sol | 8af07ce7ff299b48c89fdf165cd8efa45309a82e |
| templates/company/contracts/CompanyTemplate.sol | 6a34bac42ea02ee4abbfdcbf0437e9db0e9a1e9b |
| templates/membership/contracts/MembershipTemplate.sol | eaebf63b173efdbc8252318cbd2a29bebdd15e43 |
| templates/reputation/contracts/ReputationTemplate.sol | 9ff127c82c20cb087a66a41eba5c05fb4c8d9668 |
| templates/trust/contracts/MultiSigWallet.sol | c2448282059bb320f6ca0fa55f2038b6b22a1a2b |
| templates/trust/contracts/TrustTemplate.sol | 8748bf3bb596433517d373176d57c7e8d1561a53 |


### Contracts Description Table


|  Contract  |         Type        |       Bases      |                  |                 |
|:----------:|:-------------------:|:----------------:|:----------------:|:---------------:|
|     └      |  **Function Name**  |  **Visibility**  |  **Mutability**  |  **Modifiers**  |
||||||
| **BaseTemplate** | Implementation | APMNamehash, IsContract |||
| └ | \<Constructor\> | Public ❗️ | 🛑  | |
| └ | _createDAO | Internal 🔒 | 🛑  | |
| └ | _createPermissions | Internal 🔒 | 🛑  | |
| └ | _createPermissionForTemplate | Internal 🔒 | 🛑  | |
| └ | _removePermissionFromTemplate | Internal 🔒 | 🛑  | |
| └ | _transferRootPermissionsFromTemplateAndFinalizeDAO | Internal 🔒 | 🛑  | |
| └ | _transferRootPermissionsFromTemplateAndFinalizeDAO | Internal 🔒 | 🛑  | |
| └ | _transferPermissionFromTemplate | Internal 🔒 | 🛑  | |
| └ | _installDefaultAgentApp | Internal 🔒 | 🛑  | |
| └ | _installNonDefaultAgentApp | Internal 🔒 | 🛑  | |
| └ | _createAgentPermissions | Internal 🔒 | 🛑  | |
| └ | _installVaultApp | Internal 🔒 | 🛑  | |
| └ | _createVaultPermissions | Internal 🔒 | 🛑  | |
| └ | _installVotingApp | Internal 🔒 | 🛑  | |
| └ | _installVotingApp | Internal 🔒 | 🛑  | |
| └ | _createVotingPermissions | Internal 🔒 | 🛑  | |
| └ | _installSurveyApp | Internal 🔒 | 🛑  | |
| └ | _createSurveyPermissions | Internal 🔒 | 🛑  | |
| └ | _installPayrollApp | Internal 🔒 | 🛑  | |
| └ | _createPayrollPermissions | Internal 🔒 | 🛑  | |
| └ | _unwrapPayrollSettings | Internal 🔒 |   | |
| └ | _installFinanceApp | Internal 🔒 | 🛑  | |
| └ | _createFinancePermissions | Internal 🔒 | 🛑  | |
| └ | _installTokenManagerApp | Internal 🔒 | 🛑  | |
| └ | _createTokenManagerPermissions | Internal 🔒 | 🛑  | |
| └ | _mintTokens | Internal 🔒 | 🛑  | |
| └ | _mintTokens | Internal 🔒 | 🛑  | |
| └ | _mintTokens | Internal 🔒 | 🛑  | |
| └ | _createEvmScriptsRegistryPermissions | Internal 🔒 | 🛑  | |
| └ | _installNonDefaultApp | Internal 🔒 | 🛑  | |
| └ | _installNonDefaultApp | Internal 🔒 | 🛑  | |
| └ | _installDefaultApp | Internal 🔒 | 🛑  | |
| └ | _installDefaultApp | Internal 🔒 | 🛑  | |
| └ | _installApp | Internal 🔒 | 🛑  | |
| └ | _latestVersionAppBase | Internal 🔒 |   | |
| └ | _createToken | Internal 🔒 | 🛑  | |
| └ | _ensureMiniMeFactoryIsValid | Internal 🔒 |   | |
| └ | _registerID | Internal 🔒 | 🛑  | |
| └ | _ensureAragonIdIsValid | Internal 🔒 |   | |
| └ | _toAddress | Private 🔐 |   | |
||||||
| **TokenCache** | Implementation |  |||
| └ | _cacheToken | Internal 🔒 | 🛑  | |
| └ | _popTokenCache | Internal 🔒 | 🛑  | |
||||||
| **BareTemplate** | Implementation | BaseTemplate |||
| └ | \<Constructor\> | Public ❗️ | 🛑  | BaseTemplate |
| └ | newInstance | Public ❗️ | 🛑  |NO❗️ |
| └ | newInstance | Public ❗️ | 🛑  |NO❗️ |
||||||
| **CompanyBoardTemplate** | Implementation | BaseTemplate |||
| └ | \<Constructor\> | Public ❗️ | 🛑  | BaseTemplate |
| └ | prepareInstance | External ❗️ | 🛑  |NO❗️ |
| └ | finalizeInstance | External ❗️ | 🛑  |NO❗️ |
| └ | finalizeInstance | External ❗️ | 🛑  |NO❗️ |
| └ | _finalizeApps | Internal 🔒 | 🛑  | |
| └ | _setupVaultAndFinanceApps | Internal 🔒 | 🛑  | |
| └ | _setupPayrollApp | Internal 🔒 | 🛑  | |
| └ | _createCustomAgentPermissions | Internal 🔒 | 🛑  | |
| └ | _createCustomFinancePermissions | Internal 🔒 | 🛑  | |
| └ | _cachePreparedDao | Internal 🔒 | 🛑  | |
| └ | _popDaoCache | Internal 🔒 | 🛑  | |
| └ | _popTokenCaches | Internal 🔒 | 🛑  | |
| └ | _ensureFinalizationSettings | Private 🔐 |   | |
||||||
| **CompanyTemplate** | Implementation | BaseTemplate, TokenCache |||
| └ | \<Constructor\> | Public ❗️ | 🛑  | BaseTemplate |
| └ | newTokenAndInstance | External ❗️ | 🛑  |NO❗️ |
| └ | newToken | Public ❗️ | 🛑  |NO❗️ |
| └ | newInstance | Public ❗️ | 🛑  |NO❗️ |
| └ | newInstance | Public ❗️ | 🛑  |NO❗️ |
| └ | _setupApps | Internal 🔒 | 🛑  | |
| └ | _setupPayrollApp | Internal 🔒 | 🛑  | |
| └ | _setupPermissions | Internal 🔒 | 🛑  | |
| └ | _ensureCompanySettings | Private 🔐 |   | |
| └ | _ensureCompanySettings | Private 🔐 |   | |
||||||
| **MembershipTemplate** | Implementation | BaseTemplate, TokenCache |||
| └ | \<Constructor\> | Public ❗️ | 🛑  | BaseTemplate |
| └ | newTokenAndInstance | External ❗️ | 🛑  |NO❗️ |
| └ | newToken | Public ❗️ | 🛑  |NO❗️ |
| └ | newInstance | Public ❗️ | 🛑  |NO❗️ |
| └ | newInstance | Public ❗️ | 🛑  |NO❗️ |
| └ | _setupApps | Internal 🔒 | 🛑  | |
| └ | _setupPayrollApp | Internal 🔒 | 🛑  | |
| └ | _setupPermissions | Internal 🔒 | 🛑  | |
| └ | _ensureMembershipSettings | Private 🔐 |   | |
| └ | _ensureMembershipSettings | Private 🔐 |   | |
||||||
| **ReputationTemplate** | Implementation | BaseTemplate, TokenCache |||
| └ | \<Constructor\> | Public ❗️ | 🛑  | BaseTemplate |
| └ | newTokenAndInstance | External ❗️ | 🛑  |NO❗️ |
| └ | newToken | Public ❗️ | 🛑  |NO❗️ |
| └ | newInstance | Public ❗️ | 🛑  |NO❗️ |
| └ | newInstance | Public ❗️ | 🛑  |NO❗️ |
| └ | _setupApps | Internal 🔒 | 🛑  | |
| └ | _setupPayrollApp | Internal 🔒 | 🛑  | |
| └ | _setupPermissions | Internal 🔒 | 🛑  | |
| └ | _ensureReputationSettings | Private 🔐 |   | |
| └ | _ensureReputationSettings | Private 🔐 |   | |
||||||
| **MultiSigWallet** | Implementation |  |||
| └ | \<Fallback\> | Public ❗️ |  💵 |NO❗️ |
| └ | \<Constructor\> | Public ❗️ | 🛑  | validRequirement |
| └ | addOwner | Public ❗️ | 🛑  | onlyWallet ownerDoesNotExist notNull validRequirement |
| └ | removeOwner | Public ❗️ | 🛑  | onlyWallet ownerExists |
| └ | replaceOwner | Public ❗️ | 🛑  | onlyWallet ownerExists ownerDoesNotExist |
| └ | changeRequirement | Public ❗️ | 🛑  | onlyWallet validRequirement |
| └ | submitTransaction | Public ❗️ | 🛑  |NO❗️ |
| └ | confirmTransaction | Public ❗️ | 🛑  | ownerExists transactionExists notConfirmed |
| └ | revokeConfirmation | Public ❗️ | 🛑  | ownerExists confirmed notExecuted |
| └ | executeTransaction | Public ❗️ | 🛑  | ownerExists confirmed notExecuted |
| └ | external_call | Internal 🔒 | 🛑  | |
| └ | isConfirmed | Public ❗️ |   |NO❗️ |
| └ | addTransaction | Internal 🔒 | 🛑  | notNull |
| └ | getConfirmationCount | Public ❗️ |   |NO❗️ |
| └ | getTransactionCount | Public ❗️ |   |NO❗️ |
| └ | getOwners | Public ❗️ |   |NO❗️ |
| └ | getConfirmations | Public ❗️ |   |NO❗️ |
| └ | getTransactionIds | Public ❗️ |   |NO❗️ |
||||||
| **TrustTemplate** | Implementation | BaseTemplate |||
| └ | \<Constructor\> | Public ❗️ | 🛑  | BaseTemplate |
| └ | prepareInstance | Public ❗️ | 🛑  |NO❗️ |
| └ | setupInstance | Public ❗️ | 🛑  |NO❗️ |
| └ | setupMultiSig | Public ❗️ | 🛑  |NO❗️ |
| └ | _setupApps | Internal 🔒 | 🛑  | |
| └ | _setupMultiSig | Internal 🔒 | 🛑  | |
| └ | _createMultiSig | Internal 🔒 | 🛑  | |
| └ | _installTokenApps | Internal 🔒 | 🛑  | |
| └ | _createCustomAgentPermissions | Internal 🔒 | 🛑  | |
| └ | _createCustomTokenManagerPermissions | Internal 🔒 | 🛑  | |
| └ | _createCustomVotingPermissions | Internal 🔒 | 🛑  | |
| └ | _createMultiSigPermissions | Internal 🔒 | 🛑  | |
| └ | _storeDaoCache | Internal 🔒 | 🛑  | |
| └ | _storeAppsCache | Internal 🔒 | 🛑  | |
| └ | _cleanCache | Internal 🔒 | 🛑  | |
| └ | _hasDaoCache | Internal 🔒 |   | |
| └ | _hasAppsCache | Internal 🔒 |   | |
| └ | _getDaoCache | Internal 🔒 |   | |
| └ | _getTokensCache | Internal 🔒 |   | |
| └ | _getAppsCache | Internal 🔒 |   | |
| └ | _calculateBlockedHeirsSupply | Internal 🔒 |   | |


### Legend

|  Symbol  |  Meaning  |
|:--------:|-----------|
|    🛑    | Function can modify state |
|    💵    | Function is payable |
