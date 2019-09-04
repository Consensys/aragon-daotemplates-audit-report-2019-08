# Compiler Output

## Bare

```console

$ npx truffle compile
Compiling ./contracts/BareTemplate.sol...
Compiling ./contracts/flat_BareTemplate.sol...
Compiling ./contracts/test/TestImports.sol...
Compiling @aragon/apps-agent/contracts/Agent.sol...
Compiling @aragon/apps-agent/contracts/SignatureValidator.sol...
Compiling @aragon/apps-agent/contracts/standards/ERC1271.sol...
Compiling @aragon/apps-agent/contracts/standards/IERC165.sol...
Compiling @aragon/apps-finance/contracts/Finance.sol...
Compiling @aragon/apps-payroll/contracts/Payroll.sol...
Compiling @aragon/apps-shared-minime/contracts/ITokenController.sol...
Compiling @aragon/apps-shared-minime/contracts/MiniMeToken.sol...
Compiling @aragon/apps-survey/contracts/Survey.sol...
Compiling @aragon/apps-token-manager/contracts/TokenManager.sol...
Compiling @aragon/apps-vault/contracts/Vault.sol...
Compiling @aragon/apps-voting/contracts/Voting.sol...
Compiling @aragon/id/contracts/FIFSResolvingRegistrar.sol...
Compiling @aragon/id/contracts/IFIFSResolvingRegistrar.sol...
Compiling @aragon/id/contracts/ens/IPublicResolver.sol...
Compiling @aragon/os/contracts/acl/ACL.sol...
Compiling @aragon/os/contracts/acl/ACLSyntaxSugar.sol...
Compiling @aragon/os/contracts/acl/IACL.sol...
Compiling @aragon/os/contracts/acl/IACLOracle.sol...
Compiling @aragon/os/contracts/apm/APMNamehash.sol...
Compiling @aragon/os/contracts/apm/APMRegistry.sol...
Compiling @aragon/os/contracts/apm/Repo.sol...
Compiling @aragon/os/contracts/apps/AppProxyBase.sol...
Compiling @aragon/os/contracts/apps/AppProxyPinned.sol...
Compiling @aragon/os/contracts/apps/AppProxyUpgradeable.sol...
Compiling @aragon/os/contracts/apps/AppStorage.sol...
Compiling @aragon/os/contracts/apps/AragonApp.sol...
Compiling @aragon/os/contracts/common/Autopetrified.sol...
Compiling @aragon/os/contracts/common/ConversionHelpers.sol...
Compiling @aragon/os/contracts/common/DelegateProxy.sol...
Compiling @aragon/os/contracts/common/DepositableDelegateProxy.sol...
Compiling @aragon/os/contracts/common/DepositableStorage.sol...
Compiling @aragon/os/contracts/common/EtherTokenConstant.sol...
Compiling @aragon/os/contracts/common/IForwarder.sol...
Compiling @aragon/os/contracts/common/IVaultRecoverable.sol...
Compiling @aragon/os/contracts/common/Initializable.sol...
Compiling @aragon/os/contracts/common/IsContract.sol...
Compiling @aragon/os/contracts/common/Petrifiable.sol...
Compiling @aragon/os/contracts/common/ReentrancyGuard.sol...
Compiling @aragon/os/contracts/common/SafeERC20.sol...
Compiling @aragon/os/contracts/common/TimeHelpers.sol...
Compiling @aragon/os/contracts/common/Uint256Helpers.sol...
Compiling @aragon/os/contracts/common/UnstructuredStorage.sol...
Compiling @aragon/os/contracts/common/VaultRecoverable.sol...
Compiling @aragon/os/contracts/ens/ENSConstants.sol...
Compiling @aragon/os/contracts/ens/ENSSubdomainRegistrar.sol...
Compiling @aragon/os/contracts/evmscript/EVMScriptRegistry.sol...
Compiling @aragon/os/contracts/evmscript/EVMScriptRunner.sol...
Compiling @aragon/os/contracts/evmscript/IEVMScriptExecutor.sol...
Compiling @aragon/os/contracts/evmscript/IEVMScriptRegistry.sol...
Compiling @aragon/os/contracts/evmscript/ScriptHelpers.sol...
Compiling @aragon/os/contracts/evmscript/executors/BaseEVMScriptExecutor.sol...
Compiling @aragon/os/contracts/evmscript/executors/CallsScript.sol...
Compiling @aragon/os/contracts/factory/APMRegistryFactory.sol...
Compiling @aragon/os/contracts/factory/AppProxyFactory.sol...
Compiling @aragon/os/contracts/factory/DAOFactory.sol...
Compiling @aragon/os/contracts/factory/ENSFactory.sol...
Compiling @aragon/os/contracts/factory/EVMScriptRegistryFactory.sol...
Compiling @aragon/os/contracts/kernel/IKernel.sol...
Compiling @aragon/os/contracts/kernel/Kernel.sol...
Compiling @aragon/os/contracts/kernel/KernelConstants.sol...
Compiling @aragon/os/contracts/kernel/KernelProxy.sol...
Compiling @aragon/os/contracts/kernel/KernelStorage.sol...
Compiling @aragon/os/contracts/lib/ens/AbstractENS.sol...
Compiling @aragon/os/contracts/lib/ens/ENS.sol...
Compiling @aragon/os/contracts/lib/ens/PublicResolver.sol...
Compiling @aragon/os/contracts/lib/math/SafeMath.sol...
Compiling @aragon/os/contracts/lib/math/SafeMath64.sol...
Compiling @aragon/os/contracts/lib/misc/ERCProxy.sol...
Compiling @aragon/os/contracts/lib/token/ERC20.sol...
Compiling @aragon/ppf-contracts/contracts/IFeed.sol...
Compiling @aragon/templates-shared/contracts/BaseTemplate.sol...
Compiling @aragon/templates-shared/contracts/Migrations.sol...

Compilation warnings encountered:

@aragon/apps-shared-minime/contracts/MiniMeToken.sol:37:5: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
    function Controlled()  public { controller = msg.sender;}
    ^-------------------------------------------------------^
,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:123:5: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
    function MiniMeToken(
    ^ (Relevant source part starts here and spans across multiple lines).
,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:195:9: Warning: Use of the "var" keyword is deprecated.
        var previousBalanceFrom = balanceOfAt(_from, block.number);
        ^---------------------^
,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:209:9: Warning: Use of the "var" keyword is deprecated.
        var previousBalanceTo = balanceOfAt(_to, block.number);
        ^-------------------^
,@aragon/os/contracts/lib/ens/ENS.sol:22:48: Warning: "throw" is deprecated in favour of "revert()", "require()" and "assert()".
        if (records[node].owner != msg.sender) throw;
                                               ^---^
,@aragon/os/contracts/lib/ens/ENS.sol:29:5: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
    function ENS() public {
    ^ (Relevant source part starts here and spans across multiple lines).
,@aragon/os/contracts/lib/ens/ENS.sol:73:9: Warning: Use of the "var" keyword is deprecated.
        var subnode = keccak256(node, label);
        ^---------^
,@aragon/os/contracts/lib/ens/PublicResolver.sol:45:44: Warning: "throw" is deprecated in favour of "revert()", "require()" and "assert()".
        if (ens.owner(node) != msg.sender) throw;
                                           ^---^
,@aragon/os/contracts/lib/ens/PublicResolver.sol:53:5: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
    function PublicResolver(AbstractENS ensAddr) public {
    ^ (Relevant source part starts here and spans across multiple lines).
,@aragon/os/contracts/lib/ens/PublicResolver.sol:146:9: Warning: Use of the "var" keyword is deprecated.
        var record = records[node];
        ^--------^
,@aragon/os/contracts/lib/ens/PublicResolver.sol:166:53: Warning: "throw" is deprecated in favour of "revert()", "require()" and "assert()".
        if (((contentType - 1) & contentType) != 0) throw;
                                                    ^---^
,./templates/bare/contracts/flat_BareTemplate.sol:1781:5: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
    function Controlled()  public { controller = msg.sender;}
    ^-------------------------------------------------------^
,./templates/bare/contracts/flat_BareTemplate.sol:1867:5: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
    function MiniMeToken(
    ^ (Relevant source part starts here and spans across multiple lines).
,./templates/bare/contracts/flat_BareTemplate.sol:1939:9: Warning: Use of the "var" keyword is deprecated.
        var previousBalanceFrom = balanceOfAt(_from, block.number);
        ^---------------------^
,./templates/bare/contracts/flat_BareTemplate.sol:1953:9: Warning: Use of the "var" keyword is deprecated.
        var previousBalanceTo = balanceOfAt(_to, block.number);
        ^-------------------^
,./templates/bare/contracts/flat_BareTemplate.sol:6357:48: Warning: "throw" is deprecated in favour of "revert()", "require()" and "assert()".
        if (records[node].owner != msg.sender) throw;
                                               ^---^
,./templates/bare/contracts/flat_BareTemplate.sol:6364:5: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
    function ENS() public {
    ^ (Relevant source part starts here and spans across multiple lines).
,./templates/bare/contracts/flat_BareTemplate.sol:6408:9: Warning: Use of the "var" keyword is deprecated.
        var subnode = keccak256(node, label);
        ^---------^
,./templates/bare/contracts/flat_BareTemplate.sol:6479:44: Warning: "throw" is deprecated in favour of "revert()", "require()" and "assert()".
        if (ens.owner(node) != msg.sender) throw;
                                           ^---^
,./templates/bare/contracts/flat_BareTemplate.sol:6487:5: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
    function PublicResolver(AbstractENS ensAddr) public {
    ^ (Relevant source part starts here and spans across multiple lines).
,./templates/bare/contracts/flat_BareTemplate.sol:6580:9: Warning: Use of the "var" keyword is deprecated.
        var record = records[node];
        ^--------^
,./templates/bare/contracts/flat_BareTemplate.sol:6600:53: Warning: "throw" is deprecated in favour of "revert()", "require()" and "assert()".
        if (((contentType - 1) & contentType) != 0) throw;
                                                    ^---^
,@aragon/templates-shared/contracts/Migrations.sol:11:3: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
  function Migrations() public {
  ^ (Relevant source part starts here and spans across multiple lines).
,@aragon/os/contracts/lib/ens/ENS.sol:60:37: Warning: This declaration shadows an existing declaration.
    function setOwner(bytes32 node, address owner) only_owner(node) public {
                                    ^-----------^
@aragon/os/contracts/lib/ens/ENS.sol:36:5: The shadowed declaration is here:
    function owner(bytes32 node) public constant returns (address) {
    ^ (Relevant source part starts here and spans across multiple lines).

,@aragon/os/contracts/lib/ens/ENS.sol:72:59: Warning: This declaration shadows an existing declaration.
    function setSubnodeOwner(bytes32 node, bytes32 label, address owner) only_owner(node) public {
                                                          ^-----------^
@aragon/os/contracts/lib/ens/ENS.sol:36:5: The shadowed declaration is here:
    function owner(bytes32 node) public constant returns (address) {
    ^ (Relevant source part starts here and spans across multiple lines).

,@aragon/os/contracts/lib/ens/ENS.sol:83:40: Warning: This declaration shadows an existing declaration.
    function setResolver(bytes32 node, address resolver) only_owner(node) public {
                                       ^--------------^
@aragon/os/contracts/lib/ens/ENS.sol:43:5: The shadowed declaration is here:
    function resolver(bytes32 node) public constant returns (address) {
    ^ (Relevant source part starts here and spans across multiple lines).

,@aragon/os/contracts/lib/ens/ENS.sol:93:35: Warning: This declaration shadows an existing declaration.
    function setTTL(bytes32 node, uint64 ttl) only_owner(node) public {
                                  ^--------^
@aragon/os/contracts/lib/ens/ENS.sol:50:5: The shadowed declaration is here:
    function ttl(bytes32 node) public constant returns (uint64) {
    ^ (Relevant source part starts here and spans across multiple lines).

,@aragon/os/contracts/lib/ens/PublicResolver.sol:87:36: Warning: This declaration shadows an existing declaration.
    function setAddr(bytes32 node, address addr) only_owner(node) public {
                                   ^----------^
@aragon/os/contracts/lib/ens/PublicResolver.sol:77:5: The shadowed declaration is here:
    function addr(bytes32 node) public constant returns (address ret) {
    ^ (Relevant source part starts here and spans across multiple lines).

,@aragon/os/contracts/lib/ens/PublicResolver.sol:132:36: Warning: This declaration shadows an existing declaration.
    function setName(bytes32 node, string name) only_owner(node) public {
                                   ^---------^
@aragon/os/contracts/lib/ens/PublicResolver.sol:122:5: The shadowed declaration is here:
    function name(bytes32 node) public constant returns (string ret) {
    ^ (Relevant source part starts here and spans across multiple lines).

,@aragon/id/contracts/ens/IPublicResolver.sol:7:36: Warning: This declaration shadows an existing declaration.
    function setAddr(bytes32 node, address addr);
                                   ^----------^
@aragon/id/contracts/ens/IPublicResolver.sol:6:5: The shadowed declaration is here:
    function addr(bytes32 node) constant returns (address ret);
    ^---------------------------------------------------------^

,@aragon/id/contracts/ens/IPublicResolver.sol:9:36: Warning: This declaration shadows an existing declaration.
    function setHash(bytes32 node, bytes32 hash);
                                   ^----------^
@aragon/id/contracts/ens/IPublicResolver.sol:8:5: The shadowed declaration is here:
    function hash(bytes32 node) constant returns (bytes32 ret);
    ^---------------------------------------------------------^

,./templates/bare/contracts/flat_BareTemplate.sol:6395:37: Warning: This declaration shadows an existing declaration.
    function setOwner(bytes32 node, address owner) only_owner(node) public {
                                    ^-----------^
./templates/bare/contracts/flat_BareTemplate.sol:6371:5: The shadowed declaration is here:
    function owner(bytes32 node) public constant returns (address) {
    ^ (Relevant source part starts here and spans across multiple lines).

,./templates/bare/contracts/flat_BareTemplate.sol:6407:59: Warning: This declaration shadows an existing declaration.
    function setSubnodeOwner(bytes32 node, bytes32 label, address owner) only_owner(node) public {
                                                          ^-----------^
./templates/bare/contracts/flat_BareTemplate.sol:6371:5: The shadowed declaration is here:
    function owner(bytes32 node) public constant returns (address) {
    ^ (Relevant source part starts here and spans across multiple lines).

,./templates/bare/contracts/flat_BareTemplate.sol:6418:40: Warning: This declaration shadows an existing declaration.
    function setResolver(bytes32 node, address resolver) only_owner(node) public {
                                       ^--------------^
./templates/bare/contracts/flat_BareTemplate.sol:6378:5: The shadowed declaration is here:
    function resolver(bytes32 node) public constant returns (address) {
    ^ (Relevant source part starts here and spans across multiple lines).

,./templates/bare/contracts/flat_BareTemplate.sol:6428:35: Warning: This declaration shadows an existing declaration.
    function setTTL(bytes32 node, uint64 ttl) only_owner(node) public {
                                  ^--------^
./templates/bare/contracts/flat_BareTemplate.sol:6385:5: The shadowed declaration is here:
    function ttl(bytes32 node) public constant returns (uint64) {
    ^ (Relevant source part starts here and spans across multiple lines).

,./templates/bare/contracts/flat_BareTemplate.sol:6521:36: Warning: This declaration shadows an existing declaration.
    function setAddr(bytes32 node, address addr) only_owner(node) public {
                                   ^----------^
./templates/bare/contracts/flat_BareTemplate.sol:6511:5: The shadowed declaration is here:
    function addr(bytes32 node) public constant returns (address ret) {
    ^ (Relevant source part starts here and spans across multiple lines).

,./templates/bare/contracts/flat_BareTemplate.sol:6566:36: Warning: This declaration shadows an existing declaration.
    function setName(bytes32 node, string name) only_owner(node) public {
                                   ^---------^
./templates/bare/contracts/flat_BareTemplate.sol:6556:5: The shadowed declaration is here:
    function name(bytes32 node) public constant returns (string ret) {
    ^ (Relevant source part starts here and spans across multiple lines).

,./templates/bare/contracts/flat_BareTemplate.sol:7103:36: Warning: This declaration shadows an existing declaration.
    function setAddr(bytes32 node, address addr);
                                   ^----------^
./templates/bare/contracts/flat_BareTemplate.sol:7102:5: The shadowed declaration is here:
    function addr(bytes32 node) constant returns (address ret);
    ^---------------------------------------------------------^

,./templates/bare/contracts/flat_BareTemplate.sol:7105:36: Warning: This declaration shadows an existing declaration.
    function setHash(bytes32 node, bytes32 hash);
                                   ^----------^
./templates/bare/contracts/flat_BareTemplate.sol:7104:5: The shadowed declaration is here:
    function hash(bytes32 node) constant returns (bytes32 ret);
    ^---------------------------------------------------------^

,@aragon/apps-vault/contracts/Vault.sol:76:5: Warning: Variable is shadowed in inline assembly by an instruction of the same name
    function balance(address _token) public view returns (uint256) {
    ^ (Relevant source part starts here and spans across multiple lines).
,@aragon/apps-vault/contracts/Vault.sol:76:5: Warning: Variable is shadowed in inline assembly by an instruction of the same name
    function balance(address _token) public view returns (uint256) {
    ^ (Relevant source part starts here and spans across multiple lines).
,./templates/bare/contracts/flat_BareTemplate.sol:1356:5: Warning: Variable is shadowed in inline assembly by an instruction of the same name
    function balance(address _token) public view returns (uint256) {
    ^ (Relevant source part starts here and spans across multiple lines).
,./templates/bare/contracts/flat_BareTemplate.sol:1356:5: Warning: Variable is shadowed in inline assembly by an instruction of the same name
    function balance(address _token) public view returns (uint256) {
    ^ (Relevant source part starts here and spans across multiple lines).
,@aragon/os/contracts/acl/IACL.sol:13:5: Warning: Functions in interfaces should be declared external.
    function hasPermission(address who, address where, bytes32 what, bytes how) public view returns (bool);
    ^-----------------------------------------------------------------------------------------------------^
,@aragon/os/contracts/evmscript/IEVMScriptRegistry.sol:24:5: Warning: Functions in interfaces should be declared external.
    function getScriptExecutor(bytes script) public view returns (IEVMScriptExecutor);
    ^--------------------------------------------------------------------------------^
,@aragon/os/contracts/common/IForwarder.sol:13:5: Warning: Functions in interfaces should be declared external.
    function canForward(address sender, bytes evmCallScript) public view returns (bool);
    ^----------------------------------------------------------------------------------^
,@aragon/os/contracts/common/IForwarder.sol:17:5: Warning: Functions in interfaces should be declared external.
    function forward(bytes evmCallScript) public;
    ^-------------------------------------------^
,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:213:9: Warning: Invoking events without "emit" prefix is deprecated.
        Transfer(_from, _to, _amount);
        ^---------------------------^
,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:245:9: Warning: Invoking events without "emit" prefix is deprecated.
        Approval(msg.sender, _spender, _amount);
        ^-------------------------------------^
,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:373:9: Warning: Invoking events without "emit" prefix is deprecated.
        NewCloneToken(address(cloneToken), snapshot);
        ^------------------------------------------^
,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:392:9: Warning: Invoking events without "emit" prefix is deprecated.
        Transfer(0, _owner, _amount);
        ^--------------------------^
,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:408:9: Warning: Invoking events without "emit" prefix is deprecated.
        Transfer(_owner, 0, _amount);
        ^--------------------------^
,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:509:33: Warning: Using contract member "balance" inherited from the address type is deprecated. Convert the contract to "address" type to access the member, for example use "address(contract).balance" instead.
            controller.transfer(this.balance);
                                ^----------^
,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:516:9: Warning: Invoking events without "emit" prefix is deprecated.
        ClaimedTokens(_token, controller, balance);
        ^----------------------------------------^
,@aragon/os/contracts/lib/ens/AbstractENS.sol:7:5: Warning: Functions in interfaces should be declared external.
    function owner(bytes32 _node) public constant returns (address);
    ^--------------------------------------------------------------^
,@aragon/os/contracts/lib/ens/AbstractENS.sol:8:5: Warning: Functions in interfaces should be declared external.
    function resolver(bytes32 _node) public constant returns (address);
    ^-----------------------------------------------------------------^
,@aragon/os/contracts/lib/ens/AbstractENS.sol:9:5: Warning: Functions in interfaces should be declared external.
    function ttl(bytes32 _node) public constant returns (uint64);
    ^-----------------------------------------------------------^
,@aragon/os/contracts/lib/ens/AbstractENS.sol:10:5: Warning: Functions in interfaces should be declared external.
    function setOwner(bytes32 _node, address _owner) public;
    ^------------------------------------------------------^
,@aragon/os/contracts/lib/ens/AbstractENS.sol:11:5: Warning: Functions in interfaces should be declared external.
    function setSubnodeOwner(bytes32 _node, bytes32 label, address _owner) public;
    ^----------------------------------------------------------------------------^
,@aragon/os/contracts/lib/ens/AbstractENS.sol:12:5: Warning: Functions in interfaces should be declared external.
    function setResolver(bytes32 _node, address _resolver) public;
    ^------------------------------------------------------------^
,@aragon/os/contracts/lib/ens/AbstractENS.sol:13:5: Warning: Functions in interfaces should be declared external.
    function setTTL(bytes32 _node, uint64 _ttl) public;
    ^-------------------------------------------------^
,@aragon/os/contracts/lib/ens/ENS.sol:30:17: Warning: Decimal literal assigned to bytesXX variable will be left-aligned. Use an explicit conversion to silence this warning.
        records[0].owner = msg.sender;
                ^
,@aragon/os/contracts/lib/ens/ENS.sol:61:9: Warning: Invoking events without "emit" prefix is deprecated.
        Transfer(node, owner);
        ^-------------------^
,@aragon/os/contracts/lib/ens/ENS.sol:73:23: Warning: This function only accepts a single "bytes" argument. Please use "abi.encodePacked(...)" or a similar function to encode the data.
        var subnode = keccak256(node, label);
                      ^--------------------^
,@aragon/os/contracts/lib/ens/ENS.sol:74:9: Warning: Invoking events without "emit" prefix is deprecated.
        NewOwner(node, label, owner);
        ^--------------------------^
,@aragon/os/contracts/lib/ens/ENS.sol:84:9: Warning: Invoking events without "emit" prefix is deprecated.
        NewResolver(node, resolver);
        ^-------------------------^
,@aragon/os/contracts/lib/ens/ENS.sol:94:9: Warning: Invoking events without "emit" prefix is deprecated.
        NewTTL(node, ttl);
        ^---------------^
,@aragon/os/contracts/lib/ens/PublicResolver.sol:89:9: Warning: Invoking events without "emit" prefix is deprecated.
        AddrChanged(node, addr);
        ^---------------------^
,@aragon/os/contracts/lib/ens/PublicResolver.sol:113:9: Warning: Invoking events without "emit" prefix is deprecated.
        ContentChanged(node, hash);
        ^------------------------^
,@aragon/os/contracts/lib/ens/PublicResolver.sol:134:9: Warning: Invoking events without "emit" prefix is deprecated.
        NameChanged(node, name);
        ^---------------------^
,@aragon/os/contracts/lib/ens/PublicResolver.sol:169:9: Warning: Invoking events without "emit" prefix is deprecated.
        ABIChanged(node, contentType);
        ^---------------------------^
,@aragon/os/contracts/lib/ens/PublicResolver.sol:190:9: Warning: Invoking events without "emit" prefix is deprecated.
        PubkeyChanged(node, x, y);
        ^-----------------------^
,@aragon/os/contracts/lib/ens/PublicResolver.sol:212:9: Warning: Invoking events without "emit" prefix is deprecated.
        TextChanged(node, key, key);
        ^-------------------------^
,@aragon/id/contracts/ens/IPublicResolver.sol:5:5: Warning: Functions in interfaces should be declared external.
    function supportsInterface(bytes4 interfaceID) constant returns (bool);
    ^---------------------------------------------------------------------^
,@aragon/id/contracts/ens/IPublicResolver.sol:6:5: Warning: Functions in interfaces should be declared external.
    function addr(bytes32 node) constant returns (address ret);
    ^---------------------------------------------------------^
,@aragon/id/contracts/ens/IPublicResolver.sol:7:5: Warning: Functions in interfaces should be declared external.
    function setAddr(bytes32 node, address addr);
    ^-------------------------------------------^
,@aragon/id/contracts/ens/IPublicResolver.sol:8:5: Warning: Functions in interfaces should be declared external.
    function hash(bytes32 node) constant returns (bytes32 ret);
    ^---------------------------------------------------------^
,@aragon/id/contracts/ens/IPublicResolver.sol:9:5: Warning: Functions in interfaces should be declared external.
    function setHash(bytes32 node, bytes32 hash);
    ^-------------------------------------------^
,@aragon/id/contracts/IFIFSResolvingRegistrar.sol:8:5: Warning: Functions in interfaces should be declared external.
    function registerWithResolver(bytes32 _subnode, address _owner, IPublicResolver _resolver) public;
    ^------------------------------------------------------------------------------------------------^
,./templates/bare/contracts/flat_BareTemplate.sol:277:5: Warning: Functions in interfaces should be declared external.
    function hasPermission(address who, address where, bytes32 what, bytes how) public view returns (bool);
    ^-----------------------------------------------------------------------------------------------------^
,./templates/bare/contracts/flat_BareTemplate.sol:1044:5: Warning: Functions in interfaces should be declared external.
    function getScriptExecutor(bytes script) public view returns (IEVMScriptExecutor);
    ^--------------------------------------------------------------------------------^
,./templates/bare/contracts/flat_BareTemplate.sol:1404:5: Warning: Functions in interfaces should be declared external.
    function canForward(address sender, bytes evmCallScript) public view returns (bool);
    ^----------------------------------------------------------------------------------^
,./templates/bare/contracts/flat_BareTemplate.sol:1408:5: Warning: Functions in interfaces should be declared external.
    function forward(bytes evmCallScript) public;
    ^-------------------------------------------^
,./templates/bare/contracts/flat_BareTemplate.sol:1957:9: Warning: Invoking events without "emit" prefix is deprecated.
        Transfer(_from, _to, _amount);
        ^---------------------------^
,./templates/bare/contracts/flat_BareTemplate.sol:1989:9: Warning: Invoking events without "emit" prefix is deprecated.
        Approval(msg.sender, _spender, _amount);
        ^-------------------------------------^
,./templates/bare/contracts/flat_BareTemplate.sol:2117:9: Warning: Invoking events without "emit" prefix is deprecated.
        NewCloneToken(address(cloneToken), snapshot);
        ^------------------------------------------^
,./templates/bare/contracts/flat_BareTemplate.sol:2136:9: Warning: Invoking events without "emit" prefix is deprecated.
        Transfer(0, _owner, _amount);
        ^--------------------------^
,./templates/bare/contracts/flat_BareTemplate.sol:2152:9: Warning: Invoking events without "emit" prefix is deprecated.
        Transfer(_owner, 0, _amount);
        ^--------------------------^
,./templates/bare/contracts/flat_BareTemplate.sol:2253:33: Warning: Using contract member "balance" inherited from the address type is deprecated. Convert the contract to "address" type to access the member, for example use "address(contract).balance" instead.
            controller.transfer(this.balance);
                                ^----------^
,./templates/bare/contracts/flat_BareTemplate.sol:2260:9: Warning: Invoking events without "emit" prefix is deprecated.
        ClaimedTokens(_token, controller, balance);
        ^----------------------------------------^
,./templates/bare/contracts/flat_BareTemplate.sol:6315:5: Warning: Functions in interfaces should be declared external.
    function owner(bytes32 _node) public constant returns (address);
    ^--------------------------------------------------------------^
,./templates/bare/contracts/flat_BareTemplate.sol:6316:5: Warning: Functions in interfaces should be declared external.
    function resolver(bytes32 _node) public constant returns (address);
    ^-----------------------------------------------------------------^
,./templates/bare/contracts/flat_BareTemplate.sol:6317:5: Warning: Functions in interfaces should be declared external.
    function ttl(bytes32 _node) public constant returns (uint64);
    ^-----------------------------------------------------------^
,./templates/bare/contracts/flat_BareTemplate.sol:6318:5: Warning: Functions in interfaces should be declared external.
    function setOwner(bytes32 _node, address _owner) public;
    ^------------------------------------------------------^
,./templates/bare/contracts/flat_BareTemplate.sol:6319:5: Warning: Functions in interfaces should be declared external.
    function setSubnodeOwner(bytes32 _node, bytes32 label, address _owner) public;
    ^----------------------------------------------------------------------------^
,./templates/bare/contracts/flat_BareTemplate.sol:6320:5: Warning: Functions in interfaces should be declared external.
    function setResolver(bytes32 _node, address _resolver) public;
    ^------------------------------------------------------------^
,./templates/bare/contracts/flat_BareTemplate.sol:6321:5: Warning: Functions in interfaces should be declared external.
    function setTTL(bytes32 _node, uint64 _ttl) public;
    ^-------------------------------------------------^
,./templates/bare/contracts/flat_BareTemplate.sol:6365:17: Warning: Decimal literal assigned to bytesXX variable will be left-aligned. Use an explicit conversion to silence this warning.
        records[0].owner = msg.sender;
                ^
,./templates/bare/contracts/flat_BareTemplate.sol:6396:9: Warning: Invoking events without "emit" prefix is deprecated.
        Transfer(node, owner);
        ^-------------------^
,./templates/bare/contracts/flat_BareTemplate.sol:6408:23: Warning: This function only accepts a single "bytes" argument. Please use "abi.encodePacked(...)" or a similar function to encode the data.
        var subnode = keccak256(node, label);
                      ^--------------------^
,./templates/bare/contracts/flat_BareTemplate.sol:6409:9: Warning: Invoking events without "emit" prefix is deprecated.
        NewOwner(node, label, owner);
        ^--------------------------^
,./templates/bare/contracts/flat_BareTemplate.sol:6419:9: Warning: Invoking events without "emit" prefix is deprecated.
        NewResolver(node, resolver);
        ^-------------------------^
,./templates/bare/contracts/flat_BareTemplate.sol:6429:9: Warning: Invoking events without "emit" prefix is deprecated.
        NewTTL(node, ttl);
        ^---------------^
,./templates/bare/contracts/flat_BareTemplate.sol:6523:9: Warning: Invoking events without "emit" prefix is deprecated.
        AddrChanged(node, addr);
        ^---------------------^
,./templates/bare/contracts/flat_BareTemplate.sol:6547:9: Warning: Invoking events without "emit" prefix is deprecated.
        ContentChanged(node, hash);
        ^------------------------^
,./templates/bare/contracts/flat_BareTemplate.sol:6568:9: Warning: Invoking events without "emit" prefix is deprecated.
        NameChanged(node, name);
        ^---------------------^
,./templates/bare/contracts/flat_BareTemplate.sol:6603:9: Warning: Invoking events without "emit" prefix is deprecated.
        ABIChanged(node, contentType);
        ^---------------------------^
,./templates/bare/contracts/flat_BareTemplate.sol:6624:9: Warning: Invoking events without "emit" prefix is deprecated.
        PubkeyChanged(node, x, y);
        ^-----------------------^
,./templates/bare/contracts/flat_BareTemplate.sol:6646:9: Warning: Invoking events without "emit" prefix is deprecated.
        TextChanged(node, key, key);
        ^-------------------------^
,./templates/bare/contracts/flat_BareTemplate.sol:7101:5: Warning: Functions in interfaces should be declared external.
    function supportsInterface(bytes4 interfaceID) constant returns (bool);
    ^---------------------------------------------------------------------^
,./templates/bare/contracts/flat_BareTemplate.sol:7102:5: Warning: Functions in interfaces should be declared external.
    function addr(bytes32 node) constant returns (address ret);
    ^---------------------------------------------------------^
,./templates/bare/contracts/flat_BareTemplate.sol:7103:5: Warning: Functions in interfaces should be declared external.
    function setAddr(bytes32 node, address addr);
    ^-------------------------------------------^
,./templates/bare/contracts/flat_BareTemplate.sol:7104:5: Warning: Functions in interfaces should be declared external.
    function hash(bytes32 node) constant returns (bytes32 ret);
    ^---------------------------------------------------------^
,./templates/bare/contracts/flat_BareTemplate.sol:7105:5: Warning: Functions in interfaces should be declared external.
    function setHash(bytes32 node, bytes32 hash);
    ^-------------------------------------------^
,./templates/bare/contracts/flat_BareTemplate.sol:7116:5: Warning: Functions in interfaces should be declared external.
    function registerWithResolver(bytes32 _subnode, address _owner, IPublicResolver _resolver) public;
    ^------------------------------------------------------------------------------------------------^
,@aragon/id/contracts/FIFSResolvingRegistrar.sol:55:24: Warning: This function only accepts a single "bytes" argument. Please use "abi.encodePacked(...)" or a similar function to encode the data.
        bytes32 node = keccak256(rootNode, _subnode);
                       ^---------------------------^
,@aragon/os/contracts/common/VaultRecoverable.sol:49:34: Warning: Unused function parameter. Remove or comment out the variable name to silence this warning.
    function allowRecoverability(address token) public view returns (bool) {
                                 ^-----------^
,@aragon/id/contracts/ens/IPublicResolver.sol:5:5: Warning: No visibility specified. Defaulting to "public". In interfaces it defaults to external.
    function supportsInterface(bytes4 interfaceID) constant returns (bool);
    ^---------------------------------------------------------------------^
,@aragon/id/contracts/ens/IPublicResolver.sol:6:5: Warning: No visibility specified. Defaulting to "public". In interfaces it defaults to external.
    function addr(bytes32 node) constant returns (address ret);
    ^---------------------------------------------------------^
,@aragon/id/contracts/ens/IPublicResolver.sol:7:5: Warning: No visibility specified. Defaulting to "public". In interfaces it defaults to external.
    function setAddr(bytes32 node, address addr);
    ^-------------------------------------------^
,@aragon/id/contracts/ens/IPublicResolver.sol:8:5: Warning: No visibility specified. Defaulting to "public". In interfaces it defaults to external.
    function hash(bytes32 node) constant returns (bytes32 ret);
    ^---------------------------------------------------------^
,@aragon/id/contracts/ens/IPublicResolver.sol:9:5: Warning: No visibility specified. Defaulting to "public". In interfaces it defaults to external.
    function setHash(bytes32 node, bytes32 hash);
    ^-------------------------------------------^
,./templates/bare/contracts/flat_BareTemplate.sol:998:34: Warning: Unused function parameter. Remove or comment out the variable name to silence this warning.
    function allowRecoverability(address token) public view returns (bool) {
                                 ^-----------^
,./templates/bare/contracts/flat_BareTemplate.sol:7101:5: Warning: No visibility specified. Defaulting to "public". In interfaces it defaults to external.
    function supportsInterface(bytes4 interfaceID) constant returns (bool);
    ^---------------------------------------------------------------------^
,./templates/bare/contracts/flat_BareTemplate.sol:7102:5: Warning: No visibility specified. Defaulting to "public". In interfaces it defaults to external.
    function addr(bytes32 node) constant returns (address ret);
    ^---------------------------------------------------------^
,./templates/bare/contracts/flat_BareTemplate.sol:7103:5: Warning: No visibility specified. Defaulting to "public". In interfaces it defaults to external.
    function setAddr(bytes32 node, address addr);
    ^-------------------------------------------^
,./templates/bare/contracts/flat_BareTemplate.sol:7104:5: Warning: No visibility specified. Defaulting to "public". In interfaces it defaults to external.
    function hash(bytes32 node) constant returns (bytes32 ret);
    ^---------------------------------------------------------^
,./templates/bare/contracts/flat_BareTemplate.sol:7105:5: Warning: No visibility specified. Defaulting to "public". In interfaces it defaults to external.
    function setHash(bytes32 node, bytes32 hash);
    ^-------------------------------------------^
,./templates/bare/contracts/flat_BareTemplate.sol:3551:5: Warning: Function state mutability can be restricted to pure
    function getMaxPeriodTransitions() internal view returns (uint64) { return MAX_UINT64; }
    ^--------------------------------------------------------------------------------------^
,@aragon/apps-finance/contracts/Finance.sol:840:5: Warning: Function state mutability can be restricted to pure
    function getMaxPeriodTransitions() internal view returns (uint64) { return MAX_UINT64; }
    ^--------------------------------------------------------------------------------------^

Writing artifacts to ./build/contracts
```

## Company

```console

$ npx truffle compile
Compiling ./contracts/CompanyTemplate.sol...
Compiling ./contracts/flat_CompanyTemplate.sol...
Compiling ./contracts/test/TestImports.sol...
Compiling @aragon/apps-agent/contracts/Agent.sol...
Compiling @aragon/apps-agent/contracts/SignatureValidator.sol...
Compiling @aragon/apps-agent/contracts/standards/ERC1271.sol...
Compiling @aragon/apps-agent/contracts/standards/IERC165.sol...
Compiling @aragon/apps-finance/contracts/Finance.sol...
Compiling @aragon/apps-payroll/contracts/Payroll.sol...
Compiling @aragon/apps-shared-minime/contracts/ITokenController.sol...
Compiling @aragon/apps-shared-minime/contracts/MiniMeToken.sol...
Compiling @aragon/apps-survey/contracts/Survey.sol...
Compiling @aragon/apps-token-manager/contracts/TokenManager.sol...
Compiling @aragon/apps-vault/contracts/Vault.sol...
Compiling @aragon/apps-voting/contracts/Voting.sol...
Compiling @aragon/id/contracts/FIFSResolvingRegistrar.sol...
Compiling @aragon/id/contracts/IFIFSResolvingRegistrar.sol...
Compiling @aragon/id/contracts/ens/IPublicResolver.sol...
Compiling @aragon/os/contracts/acl/ACL.sol...
Compiling @aragon/os/contracts/acl/ACLSyntaxSugar.sol...
Compiling @aragon/os/contracts/acl/IACL.sol...
Compiling @aragon/os/contracts/acl/IACLOracle.sol...
Compiling @aragon/os/contracts/apm/APMNamehash.sol...
Compiling @aragon/os/contracts/apm/APMRegistry.sol...
Compiling @aragon/os/contracts/apm/Repo.sol...
Compiling @aragon/os/contracts/apps/AppProxyBase.sol...
Compiling @aragon/os/contracts/apps/AppProxyPinned.sol...
Compiling @aragon/os/contracts/apps/AppProxyUpgradeable.sol...
Compiling @aragon/os/contracts/apps/AppStorage.sol...
Compiling @aragon/os/contracts/apps/AragonApp.sol...
Compiling @aragon/os/contracts/common/Autopetrified.sol...
Compiling @aragon/os/contracts/common/ConversionHelpers.sol...
Compiling @aragon/os/contracts/common/DelegateProxy.sol...
Compiling @aragon/os/contracts/common/DepositableDelegateProxy.sol...
Compiling @aragon/os/contracts/common/DepositableStorage.sol...
Compiling @aragon/os/contracts/common/EtherTokenConstant.sol...
Compiling @aragon/os/contracts/common/IForwarder.sol...
Compiling @aragon/os/contracts/common/IVaultRecoverable.sol...
Compiling @aragon/os/contracts/common/Initializable.sol...
Compiling @aragon/os/contracts/common/IsContract.sol...
Compiling @aragon/os/contracts/common/Petrifiable.sol...
Compiling @aragon/os/contracts/common/ReentrancyGuard.sol...
Compiling @aragon/os/contracts/common/SafeERC20.sol...
Compiling @aragon/os/contracts/common/TimeHelpers.sol...
Compiling @aragon/os/contracts/common/Uint256Helpers.sol...
Compiling @aragon/os/contracts/common/UnstructuredStorage.sol...
Compiling @aragon/os/contracts/common/VaultRecoverable.sol...
Compiling @aragon/os/contracts/ens/ENSConstants.sol...
Compiling @aragon/os/contracts/ens/ENSSubdomainRegistrar.sol...
Compiling @aragon/os/contracts/evmscript/EVMScriptRegistry.sol...
Compiling @aragon/os/contracts/evmscript/EVMScriptRunner.sol...
Compiling @aragon/os/contracts/evmscript/IEVMScriptExecutor.sol...
Compiling @aragon/os/contracts/evmscript/IEVMScriptRegistry.sol...
Compiling @aragon/os/contracts/evmscript/ScriptHelpers.sol...
Compiling @aragon/os/contracts/evmscript/executors/BaseEVMScriptExecutor.sol...
Compiling @aragon/os/contracts/evmscript/executors/CallsScript.sol...
Compiling @aragon/os/contracts/factory/APMRegistryFactory.sol...
Compiling @aragon/os/contracts/factory/AppProxyFactory.sol...
Compiling @aragon/os/contracts/factory/DAOFactory.sol...
Compiling @aragon/os/contracts/factory/ENSFactory.sol...
Compiling @aragon/os/contracts/factory/EVMScriptRegistryFactory.sol...
Compiling @aragon/os/contracts/kernel/IKernel.sol...
Compiling @aragon/os/contracts/kernel/Kernel.sol...
Compiling @aragon/os/contracts/kernel/KernelConstants.sol...
Compiling @aragon/os/contracts/kernel/KernelProxy.sol...
Compiling @aragon/os/contracts/kernel/KernelStorage.sol...
Compiling @aragon/os/contracts/lib/ens/AbstractENS.sol...
Compiling @aragon/os/contracts/lib/ens/ENS.sol...
Compiling @aragon/os/contracts/lib/ens/PublicResolver.sol...
Compiling @aragon/os/contracts/lib/math/SafeMath.sol...
Compiling @aragon/os/contracts/lib/math/SafeMath64.sol...
Compiling @aragon/os/contracts/lib/misc/ERCProxy.sol...
Compiling @aragon/os/contracts/lib/token/ERC20.sol...
Compiling @aragon/ppf-contracts/contracts/IFeed.sol...
Compiling @aragon/templates-shared/contracts/BaseTemplate.sol...
Compiling @aragon/templates-shared/contracts/Migrations.sol...
Compiling @aragon/templates-shared/contracts/TokenCache.sol...
Compiling @aragon/templates-shared/contracts/test/mocks/ExecutionTarget.sol...

Compilation warnings encountered:

@aragon/apps-shared-minime/contracts/MiniMeToken.sol:37:5: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
    function Controlled()  public { controller = msg.sender;}
    ^-------------------------------------------------------^
,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:123:5: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
    function MiniMeToken(
    ^ (Relevant source part starts here and spans across multiple lines).
,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:195:9: Warning: Use of the "var" keyword is deprecated.
        var previousBalanceFrom = balanceOfAt(_from, block.number);
        ^---------------------^
,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:209:9: Warning: Use of the "var" keyword is deprecated.
        var previousBalanceTo = balanceOfAt(_to, block.number);
        ^-------------------^
,@aragon/os/contracts/lib/ens/ENS.sol:22:48: Warning: "throw" is deprecated in favour of "revert()", "require()" and "assert()".
        if (records[node].owner != msg.sender) throw;
                                               ^---^
,@aragon/os/contracts/lib/ens/ENS.sol:29:5: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
    function ENS() public {
    ^ (Relevant source part starts here and spans across multiple lines).
,@aragon/os/contracts/lib/ens/ENS.sol:73:9: Warning: Use of the "var" keyword is deprecated.
        var subnode = keccak256(node, label);
        ^---------^
,@aragon/os/contracts/lib/ens/PublicResolver.sol:45:44: Warning: "throw" is deprecated in favour of "revert()", "require()" and "assert()".
        if (ens.owner(node) != msg.sender) throw;
                                           ^---^
,@aragon/os/contracts/lib/ens/PublicResolver.sol:53:5: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
    function PublicResolver(AbstractENS ensAddr) public {
    ^ (Relevant source part starts here and spans across multiple lines).
,@aragon/os/contracts/lib/ens/PublicResolver.sol:146:9: Warning: Use of the "var" keyword is deprecated.
        var record = records[node];
        ^--------^
,@aragon/os/contracts/lib/ens/PublicResolver.sol:166:53: Warning: "throw" is deprecated in favour of "revert()", "require()" and "assert()".
        if (((contentType - 1) & contentType) != 0) throw;
                                                    ^---^
,./templates/company/contracts/flat_CompanyTemplate.sol:69:5: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
    function Controlled()  public { controller = msg.sender;}
    ^-------------------------------------------------------^
,./templates/company/contracts/flat_CompanyTemplate.sol:155:5: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
    function MiniMeToken(
    ^ (Relevant source part starts here and spans across multiple lines).
,./templates/company/contracts/flat_CompanyTemplate.sol:227:9: Warning: Use of the "var" keyword is deprecated.
        var previousBalanceFrom = balanceOfAt(_from, block.number);
        ^---------------------^
,./templates/company/contracts/flat_CompanyTemplate.sol:241:9: Warning: Use of the "var" keyword is deprecated.
        var previousBalanceTo = balanceOfAt(_to, block.number);
        ^-------------------^
,./templates/company/contracts/flat_CompanyTemplate.sol:6381:48: Warning: "throw" is deprecated in favour of "revert()", "require()" and "assert()".
        if (records[node].owner != msg.sender) throw;
                                               ^---^
,./templates/company/contracts/flat_CompanyTemplate.sol:6388:5: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
    function ENS() public {
    ^ (Relevant source part starts here and spans across multiple lines).
,./templates/company/contracts/flat_CompanyTemplate.sol:6432:9: Warning: Use of the "var" keyword is deprecated.
        var subnode = keccak256(node, label);
        ^---------^
,./templates/company/contracts/flat_CompanyTemplate.sol:6503:44: Warning: "throw" is deprecated in favour of "revert()", "require()" and "assert()".
        if (ens.owner(node) != msg.sender) throw;
                                           ^---^
,./templates/company/contracts/flat_CompanyTemplate.sol:6511:5: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
    function PublicResolver(AbstractENS ensAddr) public {
    ^ (Relevant source part starts here and spans across multiple lines).
,./templates/company/contracts/flat_CompanyTemplate.sol:6604:9: Warning: Use of the "var" keyword is deprecated.
        var record = records[node];
        ^--------^
,./templates/company/contracts/flat_CompanyTemplate.sol:6624:53: Warning: "throw" is deprecated in favour of "revert()", "require()" and "assert()".
        if (((contentType - 1) & contentType) != 0) throw;
                                                    ^---^
,@aragon/templates-shared/contracts/Migrations.sol:11:3: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
  function Migrations() public {
  ^ (Relevant source part starts here and spans across multiple lines).
,@aragon/os/contracts/lib/ens/ENS.sol:60:37: Warning: This declaration shadows an existing declaration.
    function setOwner(bytes32 node, address owner) only_owner(node) public {
                                    ^-----------^
@aragon/os/contracts/lib/ens/ENS.sol:36:5: The shadowed declaration is here:
    function owner(bytes32 node) public constant returns (address) {
    ^ (Relevant source part starts here and spans across multiple lines).

,@aragon/os/contracts/lib/ens/ENS.sol:72:59: Warning: This declaration shadows an existing declaration.
    function setSubnodeOwner(bytes32 node, bytes32 label, address owner) only_owner(node) public {
                                                          ^-----------^
@aragon/os/contracts/lib/ens/ENS.sol:36:5: The shadowed declaration is here:
    function owner(bytes32 node) public constant returns (address) {
    ^ (Relevant source part starts here and spans across multiple lines).

,@aragon/os/contracts/lib/ens/ENS.sol:83:40: Warning: This declaration shadows an existing declaration.
    function setResolver(bytes32 node, address resolver) only_owner(node) public {
                                       ^--------------^
@aragon/os/contracts/lib/ens/ENS.sol:43:5: The shadowed declaration is here:
    function resolver(bytes32 node) public constant returns (address) {
    ^ (Relevant source part starts here and spans across multiple lines).

,@aragon/os/contracts/lib/ens/ENS.sol:93:35: Warning: This declaration shadows an existing declaration.
    function setTTL(bytes32 node, uint64 ttl) only_owner(node) public {
                                  ^--------^
@aragon/os/contracts/lib/ens/ENS.sol:50:5: The shadowed declaration is here:
    function ttl(bytes32 node) public constant returns (uint64) {
    ^ (Relevant source part starts here and spans across multiple lines).

,@aragon/os/contracts/lib/ens/PublicResolver.sol:87:36: Warning: This declaration shadows an existing declaration.
    function setAddr(bytes32 node, address addr) only_owner(node) public {
                                   ^----------^
@aragon/os/contracts/lib/ens/PublicResolver.sol:77:5: The shadowed declaration is here:
    function addr(bytes32 node) public constant returns (address ret) {
    ^ (Relevant source part starts here and spans across multiple lines).

,@aragon/os/contracts/lib/ens/PublicResolver.sol:132:36: Warning: This declaration shadows an existing declaration.
    function setName(bytes32 node, string name) only_owner(node) public {
                                   ^---------^
@aragon/os/contracts/lib/ens/PublicResolver.sol:122:5: The shadowed declaration is here:
    function name(bytes32 node) public constant returns (string ret) {
    ^ (Relevant source part starts here and spans across multiple lines).

,@aragon/id/contracts/ens/IPublicResolver.sol:7:36: Warning: This declaration shadows an existing declaration.
    function setAddr(bytes32 node, address addr);
                                   ^----------^
@aragon/id/contracts/ens/IPublicResolver.sol:6:5: The shadowed declaration is here:
    function addr(bytes32 node) constant returns (address ret);
    ^---------------------------------------------------------^

,@aragon/id/contracts/ens/IPublicResolver.sol:9:36: Warning: This declaration shadows an existing declaration.
    function setHash(bytes32 node, bytes32 hash);
                                   ^----------^
@aragon/id/contracts/ens/IPublicResolver.sol:8:5: The shadowed declaration is here:
    function hash(bytes32 node) constant returns (bytes32 ret);
    ^---------------------------------------------------------^

,./templates/company/contracts/flat_CompanyTemplate.sol:6419:37: Warning: This declaration shadows an existing declaration.
    function setOwner(bytes32 node, address owner) only_owner(node) public {
                                    ^-----------^
./templates/company/contracts/flat_CompanyTemplate.sol:6395:5: The shadowed declaration is here:
    function owner(bytes32 node) public constant returns (address) {
    ^ (Relevant source part starts here and spans across multiple lines).

,./templates/company/contracts/flat_CompanyTemplate.sol:6431:59: Warning: This declaration shadows an existing declaration.
    function setSubnodeOwner(bytes32 node, bytes32 label, address owner) only_owner(node) public {
                                                          ^-----------^
./templates/company/contracts/flat_CompanyTemplate.sol:6395:5: The shadowed declaration is here:
    function owner(bytes32 node) public constant returns (address) {
    ^ (Relevant source part starts here and spans across multiple lines).

,./templates/company/contracts/flat_CompanyTemplate.sol:6442:40: Warning: This declaration shadows an existing declaration.
    function setResolver(bytes32 node, address resolver) only_owner(node) public {
                                       ^--------------^
./templates/company/contracts/flat_CompanyTemplate.sol:6402:5: The shadowed declaration is here:
    function resolver(bytes32 node) public constant returns (address) {
    ^ (Relevant source part starts here and spans across multiple lines).

,./templates/company/contracts/flat_CompanyTemplate.sol:6452:35: Warning: This declaration shadows an existing declaration.
    function setTTL(bytes32 node, uint64 ttl) only_owner(node) public {
                                  ^--------^
./templates/company/contracts/flat_CompanyTemplate.sol:6409:5: The shadowed declaration is here:
    function ttl(bytes32 node) public constant returns (uint64) {
    ^ (Relevant source part starts here and spans across multiple lines).

,./templates/company/contracts/flat_CompanyTemplate.sol:6545:36: Warning: This declaration shadows an existing declaration.
    function setAddr(bytes32 node, address addr) only_owner(node) public {
                                   ^----------^
./templates/company/contracts/flat_CompanyTemplate.sol:6535:5: The shadowed declaration is here:
    function addr(bytes32 node) public constant returns (address ret) {
    ^ (Relevant source part starts here and spans across multiple lines).

,./templates/company/contracts/flat_CompanyTemplate.sol:6590:36: Warning: This declaration shadows an existing declaration.
    function setName(bytes32 node, string name) only_owner(node) public {
                                   ^---------^
./templates/company/contracts/flat_CompanyTemplate.sol:6580:5: The shadowed declaration is here:
    function name(bytes32 node) public constant returns (string ret) {
    ^ (Relevant source part starts here and spans across multiple lines).

,./templates/company/contracts/flat_CompanyTemplate.sol:7127:36: Warning: This declaration shadows an existing declaration.
    function setAddr(bytes32 node, address addr);
                                   ^----------^
./templates/company/contracts/flat_CompanyTemplate.sol:7126:5: The shadowed declaration is here:
    function addr(bytes32 node) constant returns (address ret);
    ^---------------------------------------------------------^

,./templates/company/contracts/flat_CompanyTemplate.sol:7129:36: Warning: This declaration shadows an existing declaration.
    function setHash(bytes32 node, bytes32 hash);
                                   ^----------^
./templates/company/contracts/flat_CompanyTemplate.sol:7128:5: The shadowed declaration is here:
    function hash(bytes32 node) constant returns (bytes32 ret);
    ^---------------------------------------------------------^

,@aragon/apps-vault/contracts/Vault.sol:76:5: Warning: Variable is shadowed in inline assembly by an instruction of the same name
    function balance(address _token) public view returns (uint256) {
    ^ (Relevant source part starts here and spans across multiple lines).
,@aragon/apps-vault/contracts/Vault.sol:76:5: Warning: Variable is shadowed in inline assembly by an instruction of the same name
    function balance(address _token) public view returns (uint256) {
    ^ (Relevant source part starts here and spans across multiple lines).
,./templates/company/contracts/flat_CompanyTemplate.sol:1987:5: Warning: Variable is shadowed in inline assembly by an instruction of the same name
    function balance(address _token) public view returns (uint256) {
    ^ (Relevant source part starts here and spans across multiple lines).
,./templates/company/contracts/flat_CompanyTemplate.sol:1987:5: Warning: Variable is shadowed in inline assembly by an instruction of the same name
    function balance(address _token) public view returns (uint256) {
    ^ (Relevant source part starts here and spans across multiple lines).
,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:213:9: Warning: Invoking events without "emit" prefix is deprecated.
        Transfer(_from, _to, _amount);
        ^---------------------------^
,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:245:9: Warning: Invoking events without "emit" prefix is deprecated.
        Approval(msg.sender, _spender, _amount);
        ^-------------------------------------^
,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:373:9: Warning: Invoking events without "emit" prefix is deprecated.
        NewCloneToken(address(cloneToken), snapshot);
        ^------------------------------------------^
,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:392:9: Warning: Invoking events without "emit" prefix is deprecated.
        Transfer(0, _owner, _amount);
        ^--------------------------^
,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:408:9: Warning: Invoking events without "emit" prefix is deprecated.
        Transfer(_owner, 0, _amount);
        ^--------------------------^
,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:509:33: Warning: Using contract member "balance" inherited from the address type is deprecated. Convert the contract to "address" type to access the member, for example use "address(contract).balance" instead.
            controller.transfer(this.balance);
                                ^----------^
,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:516:9: Warning: Invoking events without "emit" prefix is deprecated.
        ClaimedTokens(_token, controller, balance);
        ^----------------------------------------^
,@aragon/os/contracts/acl/IACL.sol:13:5: Warning: Functions in interfaces should be declared external.
    function hasPermission(address who, address where, bytes32 what, bytes how) public view returns (bool);
    ^-----------------------------------------------------------------------------------------------------^
,@aragon/os/contracts/evmscript/IEVMScriptRegistry.sol:24:5: Warning: Functions in interfaces should be declared external.
    function getScriptExecutor(bytes script) public view returns (IEVMScriptExecutor);
    ^--------------------------------------------------------------------------------^
,@aragon/os/contracts/common/IForwarder.sol:13:5: Warning: Functions in interfaces should be declared external.
    function canForward(address sender, bytes evmCallScript) public view returns (bool);
    ^----------------------------------------------------------------------------------^
,@aragon/os/contracts/common/IForwarder.sol:17:5: Warning: Functions in interfaces should be declared external.
    function forward(bytes evmCallScript) public;
    ^-------------------------------------------^
,@aragon/os/contracts/lib/ens/AbstractENS.sol:7:5: Warning: Functions in interfaces should be declared external.
    function owner(bytes32 _node) public constant returns (address);
    ^--------------------------------------------------------------^
,@aragon/os/contracts/lib/ens/AbstractENS.sol:8:5: Warning: Functions in interfaces should be declared external.
    function resolver(bytes32 _node) public constant returns (address);
    ^-----------------------------------------------------------------^
,@aragon/os/contracts/lib/ens/AbstractENS.sol:9:5: Warning: Functions in interfaces should be declared external.
    function ttl(bytes32 _node) public constant returns (uint64);
    ^-----------------------------------------------------------^
,@aragon/os/contracts/lib/ens/AbstractENS.sol:10:5: Warning: Functions in interfaces should be declared external.
    function setOwner(bytes32 _node, address _owner) public;
    ^------------------------------------------------------^
,@aragon/os/contracts/lib/ens/AbstractENS.sol:11:5: Warning: Functions in interfaces should be declared external.
    function setSubnodeOwner(bytes32 _node, bytes32 label, address _owner) public;
    ^----------------------------------------------------------------------------^
,@aragon/os/contracts/lib/ens/AbstractENS.sol:12:5: Warning: Functions in interfaces should be declared external.
    function setResolver(bytes32 _node, address _resolver) public;
    ^------------------------------------------------------------^
,@aragon/os/contracts/lib/ens/AbstractENS.sol:13:5: Warning: Functions in interfaces should be declared external.
    function setTTL(bytes32 _node, uint64 _ttl) public;
    ^-------------------------------------------------^
,@aragon/os/contracts/lib/ens/ENS.sol:30:17: Warning: Decimal literal assigned to bytesXX variable will be left-aligned. Use an explicit conversion to silence this warning.
        records[0].owner = msg.sender;
                ^
,@aragon/os/contracts/lib/ens/ENS.sol:61:9: Warning: Invoking events without "emit" prefix is deprecated.
        Transfer(node, owner);
        ^-------------------^
,@aragon/os/contracts/lib/ens/ENS.sol:73:23: Warning: This function only accepts a single "bytes" argument. Please use "abi.encodePacked(...)" or a similar function to encode the data.
        var subnode = keccak256(node, label);
                      ^--------------------^
,@aragon/os/contracts/lib/ens/ENS.sol:74:9: Warning: Invoking events without "emit" prefix is deprecated.
        NewOwner(node, label, owner);
        ^--------------------------^
,@aragon/os/contracts/lib/ens/ENS.sol:84:9: Warning: Invoking events without "emit" prefix is deprecated.
        NewResolver(node, resolver);
        ^-------------------------^
,@aragon/os/contracts/lib/ens/ENS.sol:94:9: Warning: Invoking events without "emit" prefix is deprecated.
        NewTTL(node, ttl);
        ^---------------^
,@aragon/os/contracts/lib/ens/PublicResolver.sol:89:9: Warning: Invoking events without "emit" prefix is deprecated.
        AddrChanged(node, addr);
        ^---------------------^
,@aragon/os/contracts/lib/ens/PublicResolver.sol:113:9: Warning: Invoking events without "emit" prefix is deprecated.
        ContentChanged(node, hash);
        ^------------------------^
,@aragon/os/contracts/lib/ens/PublicResolver.sol:134:9: Warning: Invoking events without "emit" prefix is deprecated.
        NameChanged(node, name);
        ^---------------------^
,@aragon/os/contracts/lib/ens/PublicResolver.sol:169:9: Warning: Invoking events without "emit" prefix is deprecated.
        ABIChanged(node, contentType);
        ^---------------------------^
,@aragon/os/contracts/lib/ens/PublicResolver.sol:190:9: Warning: Invoking events without "emit" prefix is deprecated.
        PubkeyChanged(node, x, y);
        ^-----------------------^
,@aragon/os/contracts/lib/ens/PublicResolver.sol:212:9: Warning: Invoking events without "emit" prefix is deprecated.
        TextChanged(node, key, key);
        ^-------------------------^
,@aragon/id/contracts/ens/IPublicResolver.sol:5:5: Warning: Functions in interfaces should be declared external.
    function supportsInterface(bytes4 interfaceID) constant returns (bool);
    ^---------------------------------------------------------------------^
,@aragon/id/contracts/ens/IPublicResolver.sol:6:5: Warning: Functions in interfaces should be declared external.
    function addr(bytes32 node) constant returns (address ret);
    ^---------------------------------------------------------^
,@aragon/id/contracts/ens/IPublicResolver.sol:7:5: Warning: Functions in interfaces should be declared external.
    function setAddr(bytes32 node, address addr);
    ^-------------------------------------------^
,@aragon/id/contracts/ens/IPublicResolver.sol:8:5: Warning: Functions in interfaces should be declared external.
    function hash(bytes32 node) constant returns (bytes32 ret);
    ^---------------------------------------------------------^
,@aragon/id/contracts/ens/IPublicResolver.sol:9:5: Warning: Functions in interfaces should be declared external.
    function setHash(bytes32 node, bytes32 hash);
    ^-------------------------------------------^
,@aragon/id/contracts/IFIFSResolvingRegistrar.sol:8:5: Warning: Functions in interfaces should be declared external.
    function registerWithResolver(bytes32 _subnode, address _owner, IPublicResolver _resolver) public;
    ^------------------------------------------------------------------------------------------------^
,./templates/company/contracts/flat_CompanyTemplate.sol:245:9: Warning: Invoking events without "emit" prefix is deprecated.
        Transfer(_from, _to, _amount);
        ^---------------------------^
,./templates/company/contracts/flat_CompanyTemplate.sol:277:9: Warning: Invoking events without "emit" prefix is deprecated.
        Approval(msg.sender, _spender, _amount);
        ^-------------------------------------^
,./templates/company/contracts/flat_CompanyTemplate.sol:405:9: Warning: Invoking events without "emit" prefix is deprecated.
        NewCloneToken(address(cloneToken), snapshot);
        ^------------------------------------------^
,./templates/company/contracts/flat_CompanyTemplate.sol:424:9: Warning: Invoking events without "emit" prefix is deprecated.
        Transfer(0, _owner, _amount);
        ^--------------------------^
,./templates/company/contracts/flat_CompanyTemplate.sol:440:9: Warning: Invoking events without "emit" prefix is deprecated.
        Transfer(_owner, 0, _amount);
        ^--------------------------^
,./templates/company/contracts/flat_CompanyTemplate.sol:541:33: Warning: Using contract member "balance" inherited from the address type is deprecated. Convert the contract to "address" type to access the member, for example use "address(contract).balance" instead.
            controller.transfer(this.balance);
                                ^----------^
,./templates/company/contracts/flat_CompanyTemplate.sol:548:9: Warning: Invoking events without "emit" prefix is deprecated.
        ClaimedTokens(_token, controller, balance);
        ^----------------------------------------^
,./templates/company/contracts/flat_CompanyTemplate.sol:908:5: Warning: Functions in interfaces should be declared external.
    function hasPermission(address who, address where, bytes32 what, bytes how) public view returns (bool);
    ^-----------------------------------------------------------------------------------------------------^
,./templates/company/contracts/flat_CompanyTemplate.sol:1675:5: Warning: Functions in interfaces should be declared external.
    function getScriptExecutor(bytes script) public view returns (IEVMScriptExecutor);
    ^--------------------------------------------------------------------------------^
,./templates/company/contracts/flat_CompanyTemplate.sol:2035:5: Warning: Functions in interfaces should be declared external.
    function canForward(address sender, bytes evmCallScript) public view returns (bool);
    ^----------------------------------------------------------------------------------^
,./templates/company/contracts/flat_CompanyTemplate.sol:2039:5: Warning: Functions in interfaces should be declared external.
    function forward(bytes evmCallScript) public;
    ^-------------------------------------------^
,./templates/company/contracts/flat_CompanyTemplate.sol:6339:5: Warning: Functions in interfaces should be declared external.
    function owner(bytes32 _node) public constant returns (address);
    ^--------------------------------------------------------------^
,./templates/company/contracts/flat_CompanyTemplate.sol:6340:5: Warning: Functions in interfaces should be declared external.
    function resolver(bytes32 _node) public constant returns (address);
    ^-----------------------------------------------------------------^
,./templates/company/contracts/flat_CompanyTemplate.sol:6341:5: Warning: Functions in interfaces should be declared external.
    function ttl(bytes32 _node) public constant returns (uint64);
    ^-----------------------------------------------------------^
,./templates/company/contracts/flat_CompanyTemplate.sol:6342:5: Warning: Functions in interfaces should be declared external.
    function setOwner(bytes32 _node, address _owner) public;
    ^------------------------------------------------------^
,./templates/company/contracts/flat_CompanyTemplate.sol:6343:5: Warning: Functions in interfaces should be declared external.
    function setSubnodeOwner(bytes32 _node, bytes32 label, address _owner) public;
    ^----------------------------------------------------------------------------^
,./templates/company/contracts/flat_CompanyTemplate.sol:6344:5: Warning: Functions in interfaces should be declared external.
    function setResolver(bytes32 _node, address _resolver) public;
    ^------------------------------------------------------------^
,./templates/company/contracts/flat_CompanyTemplate.sol:6345:5: Warning: Functions in interfaces should be declared external.
    function setTTL(bytes32 _node, uint64 _ttl) public;
    ^-------------------------------------------------^
,./templates/company/contracts/flat_CompanyTemplate.sol:6389:17: Warning: Decimal literal assigned to bytesXX variable will be left-aligned. Use an explicit conversion to silence this warning.
        records[0].owner = msg.sender;
                ^
,./templates/company/contracts/flat_CompanyTemplate.sol:6420:9: Warning: Invoking events without "emit" prefix is deprecated.
        Transfer(node, owner);
        ^-------------------^
,./templates/company/contracts/flat_CompanyTemplate.sol:6432:23: Warning: This function only accepts a single "bytes" argument. Please use "abi.encodePacked(...)" or a similar function to encode the data.
        var subnode = keccak256(node, label);
                      ^--------------------^
,./templates/company/contracts/flat_CompanyTemplate.sol:6433:9: Warning: Invoking events without "emit" prefix is deprecated.
        NewOwner(node, label, owner);
        ^--------------------------^
,./templates/company/contracts/flat_CompanyTemplate.sol:6443:9: Warning: Invoking events without "emit" prefix is deprecated.
        NewResolver(node, resolver);
        ^-------------------------^
,./templates/company/contracts/flat_CompanyTemplate.sol:6453:9: Warning: Invoking events without "emit" prefix is deprecated.
        NewTTL(node, ttl);
        ^---------------^
,./templates/company/contracts/flat_CompanyTemplate.sol:6547:9: Warning: Invoking events without "emit" prefix is deprecated.
        AddrChanged(node, addr);
        ^---------------------^
,./templates/company/contracts/flat_CompanyTemplate.sol:6571:9: Warning: Invoking events without "emit" prefix is deprecated.
        ContentChanged(node, hash);
        ^------------------------^
,./templates/company/contracts/flat_CompanyTemplate.sol:6592:9: Warning: Invoking events without "emit" prefix is deprecated.
        NameChanged(node, name);
        ^---------------------^
,./templates/company/contracts/flat_CompanyTemplate.sol:6627:9: Warning: Invoking events without "emit" prefix is deprecated.
        ABIChanged(node, contentType);
        ^---------------------------^
,./templates/company/contracts/flat_CompanyTemplate.sol:6648:9: Warning: Invoking events without "emit" prefix is deprecated.
        PubkeyChanged(node, x, y);
        ^-----------------------^
,./templates/company/contracts/flat_CompanyTemplate.sol:6670:9: Warning: Invoking events without "emit" prefix is deprecated.
        TextChanged(node, key, key);
        ^-------------------------^
,./templates/company/contracts/flat_CompanyTemplate.sol:7125:5: Warning: Functions in interfaces should be declared external.
    function supportsInterface(bytes4 interfaceID) constant returns (bool);
    ^---------------------------------------------------------------------^
,./templates/company/contracts/flat_CompanyTemplate.sol:7126:5: Warning: Functions in interfaces should be declared external.
    function addr(bytes32 node) constant returns (address ret);
    ^---------------------------------------------------------^
,./templates/company/contracts/flat_CompanyTemplate.sol:7127:5: Warning: Functions in interfaces should be declared external.
    function setAddr(bytes32 node, address addr);
    ^-------------------------------------------^
,./templates/company/contracts/flat_CompanyTemplate.sol:7128:5: Warning: Functions in interfaces should be declared external.
    function hash(bytes32 node) constant returns (bytes32 ret);
    ^---------------------------------------------------------^
,./templates/company/contracts/flat_CompanyTemplate.sol:7129:5: Warning: Functions in interfaces should be declared external.
    function setHash(bytes32 node, bytes32 hash);
    ^-------------------------------------------^
,./templates/company/contracts/flat_CompanyTemplate.sol:7140:5: Warning: Functions in interfaces should be declared external.
    function registerWithResolver(bytes32 _subnode, address _owner, IPublicResolver _resolver) public;
    ^------------------------------------------------------------------------------------------------^
,@aragon/id/contracts/FIFSResolvingRegistrar.sol:55:24: Warning: This function only accepts a single "bytes" argument. Please use "abi.encodePacked(...)" or a similar function to encode the data.
        bytes32 node = keccak256(rootNode, _subnode);
                       ^---------------------------^
,@aragon/os/contracts/common/VaultRecoverable.sol:49:34: Warning: Unused function parameter. Remove or comment out the variable name to silence this warning.
    function allowRecoverability(address token) public view returns (bool) {
                                 ^-----------^
,@aragon/id/contracts/ens/IPublicResolver.sol:5:5: Warning: No visibility specified. Defaulting to "public". In interfaces it defaults to external.
    function supportsInterface(bytes4 interfaceID) constant returns (bool);
    ^---------------------------------------------------------------------^
,@aragon/id/contracts/ens/IPublicResolver.sol:6:5: Warning: No visibility specified. Defaulting to "public". In interfaces it defaults to external.
    function addr(bytes32 node) constant returns (address ret);
    ^---------------------------------------------------------^
,@aragon/id/contracts/ens/IPublicResolver.sol:7:5: Warning: No visibility specified. Defaulting to "public". In interfaces it defaults to external.
    function setAddr(bytes32 node, address addr);
    ^-------------------------------------------^
,@aragon/id/contracts/ens/IPublicResolver.sol:8:5: Warning: No visibility specified. Defaulting to "public". In interfaces it defaults to external.
    function hash(bytes32 node) constant returns (bytes32 ret);
    ^---------------------------------------------------------^
,@aragon/id/contracts/ens/IPublicResolver.sol:9:5: Warning: No visibility specified. Defaulting to "public". In interfaces it defaults to external.
    function setHash(bytes32 node, bytes32 hash);
    ^-------------------------------------------^
,./templates/company/contracts/flat_CompanyTemplate.sol:1629:34: Warning: Unused function parameter. Remove or comment out the variable name to silence this warning.
    function allowRecoverability(address token) public view returns (bool) {
                                 ^-----------^
,./templates/company/contracts/flat_CompanyTemplate.sol:7125:5: Warning: No visibility specified. Defaulting to "public". In interfaces it defaults to external.
    function supportsInterface(bytes4 interfaceID) constant returns (bool);
    ^---------------------------------------------------------------------^
,./templates/company/contracts/flat_CompanyTemplate.sol:7126:5: Warning: No visibility specified. Defaulting to "public". In interfaces it defaults to external.
    function addr(bytes32 node) constant returns (address ret);
    ^---------------------------------------------------------^
,./templates/company/contracts/flat_CompanyTemplate.sol:7127:5: Warning: No visibility specified. Defaulting to "public". In interfaces it defaults to external.
    function setAddr(bytes32 node, address addr);
    ^-------------------------------------------^
,./templates/company/contracts/flat_CompanyTemplate.sol:7128:5: Warning: No visibility specified. Defaulting to "public". In interfaces it defaults to external.
    function hash(bytes32 node) constant returns (bytes32 ret);
    ^---------------------------------------------------------^
,./templates/company/contracts/flat_CompanyTemplate.sol:7129:5: Warning: No visibility specified. Defaulting to "public". In interfaces it defaults to external.
    function setHash(bytes32 node, bytes32 hash);
    ^-------------------------------------------^
,./templates/company/contracts/flat_CompanyTemplate.sol:3575:5: Warning: Function state mutability can be restricted to pure
    function getMaxPeriodTransitions() internal view returns (uint64) { return MAX_UINT64; }
    ^--------------------------------------------------------------------------------------^
,@aragon/apps-finance/contracts/Finance.sol:840:5: Warning: Function state mutability can be restricted to pure
    function getMaxPeriodTransitions() internal view returns (uint64) { return MAX_UINT64; }
    ^--------------------------------------------------------------------------------------^

Writing artifacts to ./build/contracts
```

## Company-Board

```console
$ npx truffle compile

Compiling ./contracts/CompanyBoardTemplate.sol...
Compiling ./contracts/flat_CompanyBoardTemplate.sol...
Compiling ./contracts/test/TestImports.sol...
Compiling @aragon/apps-agent/contracts/Agent.sol...
Compiling @aragon/apps-agent/contracts/SignatureValidator.sol...
Compiling @aragon/apps-agent/contracts/standards/ERC1271.sol...
Compiling @aragon/apps-agent/contracts/standards/IERC165.sol...
Compiling @aragon/apps-finance/contracts/Finance.sol...
Compiling @aragon/apps-payroll/contracts/Payroll.sol...
Compiling @aragon/apps-shared-minime/contracts/ITokenController.sol...
Compiling @aragon/apps-shared-minime/contracts/MiniMeToken.sol...
Compiling @aragon/apps-survey/contracts/Survey.sol...
Compiling @aragon/apps-token-manager/contracts/TokenManager.sol...
Compiling @aragon/apps-vault/contracts/Vault.sol...
Compiling @aragon/apps-voting/contracts/Voting.sol...
Compiling @aragon/id/contracts/FIFSResolvingRegistrar.sol...
Compiling @aragon/id/contracts/IFIFSResolvingRegistrar.sol...
Compiling @aragon/id/contracts/ens/IPublicResolver.sol...
Compiling @aragon/os/contracts/acl/ACL.sol...
Compiling @aragon/os/contracts/acl/ACLSyntaxSugar.sol...
Compiling @aragon/os/contracts/acl/IACL.sol...
Compiling @aragon/os/contracts/acl/IACLOracle.sol...
Compiling @aragon/os/contracts/apm/APMNamehash.sol...
Compiling @aragon/os/contracts/apm/APMRegistry.sol...
Compiling @aragon/os/contracts/apm/Repo.sol...
Compiling @aragon/os/contracts/apps/AppProxyBase.sol...
Compiling @aragon/os/contracts/apps/AppProxyPinned.sol...
Compiling @aragon/os/contracts/apps/AppProxyUpgradeable.sol...
Compiling @aragon/os/contracts/apps/AppStorage.sol...
Compiling @aragon/os/contracts/apps/AragonApp.sol...
Compiling @aragon/os/contracts/common/Autopetrified.sol...
Compiling @aragon/os/contracts/common/ConversionHelpers.sol...
Compiling @aragon/os/contracts/common/DelegateProxy.sol...
Compiling @aragon/os/contracts/common/DepositableDelegateProxy.sol...
Compiling @aragon/os/contracts/common/DepositableStorage.sol...
Compiling @aragon/os/contracts/common/EtherTokenConstant.sol...
Compiling @aragon/os/contracts/common/IForwarder.sol...
Compiling @aragon/os/contracts/common/IVaultRecoverable.sol...
Compiling @aragon/os/contracts/common/Initializable.sol...
Compiling @aragon/os/contracts/common/IsContract.sol...
Compiling @aragon/os/contracts/common/Petrifiable.sol...
Compiling @aragon/os/contracts/common/ReentrancyGuard.sol...
Compiling @aragon/os/contracts/common/SafeERC20.sol...
Compiling @aragon/os/contracts/common/TimeHelpers.sol...
Compiling @aragon/os/contracts/common/Uint256Helpers.sol...
Compiling @aragon/os/contracts/common/UnstructuredStorage.sol...
Compiling @aragon/os/contracts/common/VaultRecoverable.sol...
Compiling @aragon/os/contracts/ens/ENSConstants.sol...
Compiling @aragon/os/contracts/ens/ENSSubdomainRegistrar.sol...
Compiling @aragon/os/contracts/evmscript/EVMScriptRegistry.sol...
Compiling @aragon/os/contracts/evmscript/EVMScriptRunner.sol...
Compiling @aragon/os/contracts/evmscript/IEVMScriptExecutor.sol...
Compiling @aragon/os/contracts/evmscript/IEVMScriptRegistry.sol...
Compiling @aragon/os/contracts/evmscript/ScriptHelpers.sol...
Compiling @aragon/os/contracts/evmscript/executors/BaseEVMScriptExecutor.sol...
Compiling @aragon/os/contracts/evmscript/executors/CallsScript.sol...
Compiling @aragon/os/contracts/factory/APMRegistryFactory.sol...
Compiling @aragon/os/contracts/factory/AppProxyFactory.sol...
Compiling @aragon/os/contracts/factory/DAOFactory.sol...
Compiling @aragon/os/contracts/factory/ENSFactory.sol...
Compiling @aragon/os/contracts/factory/EVMScriptRegistryFactory.sol...
Compiling @aragon/os/contracts/kernel/IKernel.sol...
Compiling @aragon/os/contracts/kernel/Kernel.sol...
Compiling @aragon/os/contracts/kernel/KernelConstants.sol...
Compiling @aragon/os/contracts/kernel/KernelProxy.sol...
Compiling @aragon/os/contracts/kernel/KernelStorage.sol...
Compiling @aragon/os/contracts/lib/ens/AbstractENS.sol...
Compiling @aragon/os/contracts/lib/ens/ENS.sol...
Compiling @aragon/os/contracts/lib/ens/PublicResolver.sol...
Compiling @aragon/os/contracts/lib/math/SafeMath.sol...
Compiling @aragon/os/contracts/lib/math/SafeMath64.sol...
Compiling @aragon/os/contracts/lib/misc/ERCProxy.sol...
Compiling @aragon/os/contracts/lib/token/ERC20.sol...
Compiling @aragon/ppf-contracts/contracts/IFeed.sol...
Compiling @aragon/templates-shared/contracts/BaseTemplate.sol...
Compiling @aragon/templates-shared/contracts/Migrations.sol...
Compiling @aragon/templates-shared/contracts/test/mocks/ExecutionTarget.sol...

Compilation warnings encountered:

@aragon/apps-shared-minime/contracts/MiniMeToken.sol:37:5: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
    function Controlled()  public { controller = msg.sender;}
    ^-------------------------------------------------------^
,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:123:5: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
    function MiniMeToken(
    ^ (Relevant source part starts here and spans across multiple lines).
,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:195:9: Warning: Use of the "var" keyword is deprecated.
        var previousBalanceFrom = balanceOfAt(_from, block.number);
        ^---------------------^
,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:209:9: Warning: Use of the "var" keyword is deprecated.
        var previousBalanceTo = balanceOfAt(_to, block.number);
        ^-------------------^
,@aragon/os/contracts/lib/ens/ENS.sol:22:48: Warning: "throw" is deprecated in favour of "revert()", "require()" and "assert()".
        if (records[node].owner != msg.sender) throw;
                                               ^---^
,@aragon/os/contracts/lib/ens/ENS.sol:29:5: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
    function ENS() public {
    ^ (Relevant source part starts here and spans across multiple lines).
,@aragon/os/contracts/lib/ens/ENS.sol:73:9: Warning: Use of the "var" keyword is deprecated.
        var subnode = keccak256(node, label);
        ^---------^
,@aragon/os/contracts/lib/ens/PublicResolver.sol:45:44: Warning: "throw" is deprecated in favour of "revert()", "require()" and "assert()".
        if (ens.owner(node) != msg.sender) throw;
                                           ^---^
,@aragon/os/contracts/lib/ens/PublicResolver.sol:53:5: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
    function PublicResolver(AbstractENS ensAddr) public {
    ^ (Relevant source part starts here and spans across multiple lines).
,@aragon/os/contracts/lib/ens/PublicResolver.sol:146:9: Warning: Use of the "var" keyword is deprecated.
        var record = records[node];
        ^--------^
,@aragon/os/contracts/lib/ens/PublicResolver.sol:166:53: Warning: "throw" is deprecated in favour of "revert()", "require()" and "assert()".
        if (((contentType - 1) & contentType) != 0) throw;
                                                    ^---^
,./templates/company-board/contracts/flat_CompanyBoardTemplate.sol:1781:5: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
    function Controlled()  public { controller = msg.sender;}
    ^-------------------------------------------------------^
,./templates/company-board/contracts/flat_CompanyBoardTemplate.sol:1867:5: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
    function MiniMeToken(
    ^ (Relevant source part starts here and spans across multiple lines).
,./templates/company-board/contracts/flat_CompanyBoardTemplate.sol:1939:9: Warning: Use of the "var" keyword is deprecated.
        var previousBalanceFrom = balanceOfAt(_from, block.number);
        ^---------------------^
,./templates/company-board/contracts/flat_CompanyBoardTemplate.sol:1953:9: Warning: Use of the "var" keyword is deprecated.
        var previousBalanceTo = balanceOfAt(_to, block.number);
        ^-------------------^
,./templates/company-board/contracts/flat_CompanyBoardTemplate.sol:6357:48: Warning: "throw" is deprecated in favour of "revert()", "require()" and "assert()".
        if (records[node].owner != msg.sender) throw;
                                               ^---^
,./templates/company-board/contracts/flat_CompanyBoardTemplate.sol:6364:5: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
    function ENS() public {
    ^ (Relevant source part starts here and spans across multiple lines).
,./templates/company-board/contracts/flat_CompanyBoardTemplate.sol:6408:9: Warning: Use of the "var" keyword is deprecated.
        var subnode = keccak256(node, label);
        ^---------^
,./templates/company-board/contracts/flat_CompanyBoardTemplate.sol:6479:44: Warning: "throw" is deprecated in favour of "revert()", "require()" and "assert()".
        if (ens.owner(node) != msg.sender) throw;
                                           ^---^
,./templates/company-board/contracts/flat_CompanyBoardTemplate.sol:6487:5: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
    function PublicResolver(AbstractENS ensAddr) public {
    ^ (Relevant source part starts here and spans across multiple lines).
,./templates/company-board/contracts/flat_CompanyBoardTemplate.sol:6580:9: Warning: Use of the "var" keyword is deprecated.
        var record = records[node];
        ^--------^
,./templates/company-board/contracts/flat_CompanyBoardTemplate.sol:6600:53: Warning: "throw" is deprecated in favour of "revert()", "require()" and "assert()".
        if (((contentType - 1) & contentType) != 0) throw;
                                                    ^---^
,@aragon/templates-shared/contracts/Migrations.sol:11:3: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
  function Migrations() public {
  ^ (Relevant source part starts here and spans across multiple lines).
,@aragon/os/contracts/lib/ens/ENS.sol:60:37: Warning: This declaration shadows an existing declaration.
    function setOwner(bytes32 node, address owner) only_owner(node) public {
                                    ^-----------^
@aragon/os/contracts/lib/ens/ENS.sol:36:5: The shadowed declaration is here:
    function owner(bytes32 node) public constant returns (address) {
    ^ (Relevant source part starts here and spans across multiple lines).

,@aragon/os/contracts/lib/ens/ENS.sol:72:59: Warning: This declaration shadows an existing declaration.
    function setSubnodeOwner(bytes32 node, bytes32 label, address owner) only_owner(node) public {
                                                          ^-----------^
@aragon/os/contracts/lib/ens/ENS.sol:36:5: The shadowed declaration is here:
    function owner(bytes32 node) public constant returns (address) {
    ^ (Relevant source part starts here and spans across multiple lines).

,@aragon/os/contracts/lib/ens/ENS.sol:83:40: Warning: This declaration shadows an existing declaration.
    function setResolver(bytes32 node, address resolver) only_owner(node) public {
                                       ^--------------^
@aragon/os/contracts/lib/ens/ENS.sol:43:5: The shadowed declaration is here:
    function resolver(bytes32 node) public constant returns (address) {
    ^ (Relevant source part starts here and spans across multiple lines).

,@aragon/os/contracts/lib/ens/ENS.sol:93:35: Warning: This declaration shadows an existing declaration.
    function setTTL(bytes32 node, uint64 ttl) only_owner(node) public {
                                  ^--------^
@aragon/os/contracts/lib/ens/ENS.sol:50:5: The shadowed declaration is here:
    function ttl(bytes32 node) public constant returns (uint64) {
    ^ (Relevant source part starts here and spans across multiple lines).

,@aragon/os/contracts/lib/ens/PublicResolver.sol:87:36: Warning: This declaration shadows an existing declaration.
    function setAddr(bytes32 node, address addr) only_owner(node) public {
                                   ^----------^
@aragon/os/contracts/lib/ens/PublicResolver.sol:77:5: The shadowed declaration is here:
    function addr(bytes32 node) public constant returns (address ret) {
    ^ (Relevant source part starts here and spans across multiple lines).

,@aragon/os/contracts/lib/ens/PublicResolver.sol:132:36: Warning: This declaration shadows an existing declaration.
    function setName(bytes32 node, string name) only_owner(node) public {
                                   ^---------^
@aragon/os/contracts/lib/ens/PublicResolver.sol:122:5: The shadowed declaration is here:
    function name(bytes32 node) public constant returns (string ret) {
    ^ (Relevant source part starts here and spans across multiple lines).

,@aragon/id/contracts/ens/IPublicResolver.sol:7:36: Warning: This declaration shadows an existing declaration.
    function setAddr(bytes32 node, address addr);
                                   ^----------^
@aragon/id/contracts/ens/IPublicResolver.sol:6:5: The shadowed declaration is here:
    function addr(bytes32 node) constant returns (address ret);
    ^---------------------------------------------------------^

,@aragon/id/contracts/ens/IPublicResolver.sol:9:36: Warning: This declaration shadows an existing declaration.
    function setHash(bytes32 node, bytes32 hash);
                                   ^----------^
@aragon/id/contracts/ens/IPublicResolver.sol:8:5: The shadowed declaration is here:
    function hash(bytes32 node) constant returns (bytes32 ret);
    ^---------------------------------------------------------^

,./templates/company-board/contracts/flat_CompanyBoardTemplate.sol:6395:37: Warning: This declaration shadows an existing declaration.
    function setOwner(bytes32 node, address owner) only_owner(node) public {
                                    ^-----------^
./templates/company-board/contracts/flat_CompanyBoardTemplate.sol:6371:5: The shadowed declaration is here:
    function owner(bytes32 node) public constant returns (address) {
    ^ (Relevant source part starts here and spans across multiple lines).

,./templates/company-board/contracts/flat_CompanyBoardTemplate.sol:6407:59: Warning: This declaration shadows an existing declaration.
    function setSubnodeOwner(bytes32 node, bytes32 label, address owner) only_owner(node) public {
                                                          ^-----------^
./templates/company-board/contracts/flat_CompanyBoardTemplate.sol:6371:5: The shadowed declaration is here:
    function owner(bytes32 node) public constant returns (address) {
    ^ (Relevant source part starts here and spans across multiple lines).

,./templates/company-board/contracts/flat_CompanyBoardTemplate.sol:6418:40: Warning: This declaration shadows an existing declaration.
    function setResolver(bytes32 node, address resolver) only_owner(node) public {
                                       ^--------------^
./templates/company-board/contracts/flat_CompanyBoardTemplate.sol:6378:5: The shadowed declaration is here:
    function resolver(bytes32 node) public constant returns (address) {
    ^ (Relevant source part starts here and spans across multiple lines).

,./templates/company-board/contracts/flat_CompanyBoardTemplate.sol:6428:35: Warning: This declaration shadows an existing declaration.
    function setTTL(bytes32 node, uint64 ttl) only_owner(node) public {
                                  ^--------^
./templates/company-board/contracts/flat_CompanyBoardTemplate.sol:6385:5: The shadowed declaration is here:
    function ttl(bytes32 node) public constant returns (uint64) {
    ^ (Relevant source part starts here and spans across multiple lines).

,./templates/company-board/contracts/flat_CompanyBoardTemplate.sol:6521:36: Warning: This declaration shadows an existing declaration.
    function setAddr(bytes32 node, address addr) only_owner(node) public {
                                   ^----------^
./templates/company-board/contracts/flat_CompanyBoardTemplate.sol:6511:5: The shadowed declaration is here:
    function addr(bytes32 node) public constant returns (address ret) {
    ^ (Relevant source part starts here and spans across multiple lines).

,./templates/company-board/contracts/flat_CompanyBoardTemplate.sol:6566:36: Warning: This declaration shadows an existing declaration.
    function setName(bytes32 node, string name) only_owner(node) public {
                                   ^---------^
./templates/company-board/contracts/flat_CompanyBoardTemplate.sol:6556:5: The shadowed declaration is here:
    function name(bytes32 node) public constant returns (string ret) {
    ^ (Relevant source part starts here and spans across multiple lines).

,./templates/company-board/contracts/flat_CompanyBoardTemplate.sol:7103:36: Warning: This declaration shadows an existing declaration.
    function setAddr(bytes32 node, address addr);
                                   ^----------^
./templates/company-board/contracts/flat_CompanyBoardTemplate.sol:7102:5: The shadowed declaration is here:
    function addr(bytes32 node) constant returns (address ret);
    ^---------------------------------------------------------^

,./templates/company-board/contracts/flat_CompanyBoardTemplate.sol:7105:36: Warning: This declaration shadows an existing declaration.
    function setHash(bytes32 node, bytes32 hash);
                                   ^----------^
./templates/company-board/contracts/flat_CompanyBoardTemplate.sol:7104:5: The shadowed declaration is here:
    function hash(bytes32 node) constant returns (bytes32 ret);
    ^---------------------------------------------------------^

,@aragon/apps-vault/contracts/Vault.sol:76:5: Warning: Variable is shadowed in inline assembly by an instruction of the same name
    function balance(address _token) public view returns (uint256) {
    ^ (Relevant source part starts here and spans across multiple lines).
,@aragon/apps-vault/contracts/Vault.sol:76:5: Warning: Variable is shadowed in inline assembly by an instruction of the same name
    function balance(address _token) public view returns (uint256) {
    ^ (Relevant source part starts here and spans across multiple lines).
,./templates/company-board/contracts/flat_CompanyBoardTemplate.sol:1356:5: Warning: Variable is shadowed in inline assembly by an instruction of the same name
    function balance(address _token) public view returns (uint256) {
    ^ (Relevant source part starts here and spans across multiple lines).
,./templates/company-board/contracts/flat_CompanyBoardTemplate.sol:1356:5: Warning: Variable is shadowed in inline assembly by an instruction of the same name
    function balance(address _token) public view returns (uint256) {
    ^ (Relevant source part starts here and spans across multiple lines).
,@aragon/os/contracts/acl/IACL.sol:13:5: Warning: Functions in interfaces should be declared external.
    function hasPermission(address who, address where, bytes32 what, bytes how) public view returns (bool);
    ^-----------------------------------------------------------------------------------------------------^
,@aragon/os/contracts/evmscript/IEVMScriptRegistry.sol:24:5: Warning: Functions in interfaces should be declared external.
    function getScriptExecutor(bytes script) public view returns (IEVMScriptExecutor);
    ^--------------------------------------------------------------------------------^
,@aragon/os/contracts/common/IForwarder.sol:13:5: Warning: Functions in interfaces should be declared external.
    function canForward(address sender, bytes evmCallScript) public view returns (bool);
    ^----------------------------------------------------------------------------------^
,@aragon/os/contracts/common/IForwarder.sol:17:5: Warning: Functions in interfaces should be declared external.
    function forward(bytes evmCallScript) public;
    ^-------------------------------------------^
,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:213:9: Warning: Invoking events without "emit" prefix is deprecated.
        Transfer(_from, _to, _amount);
        ^---------------------------^
,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:245:9: Warning: Invoking events without "emit" prefix is deprecated.
        Approval(msg.sender, _spender, _amount);
        ^-------------------------------------^
,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:373:9: Warning: Invoking events without "emit" prefix is deprecated.
        NewCloneToken(address(cloneToken), snapshot);
        ^------------------------------------------^
,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:392:9: Warning: Invoking events without "emit" prefix is deprecated.
        Transfer(0, _owner, _amount);
        ^--------------------------^
,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:408:9: Warning: Invoking events without "emit" prefix is deprecated.
        Transfer(_owner, 0, _amount);
        ^--------------------------^
,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:509:33: Warning: Using contract member "balance" inherited from the address type is deprecated. Convert the contract to "address" type to access the member, for example use "address(contract).balance" instead.
            controller.transfer(this.balance);
                                ^----------^
,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:516:9: Warning: Invoking events without "emit" prefix is deprecated.
        ClaimedTokens(_token, controller, balance);
        ^----------------------------------------^
,@aragon/os/contracts/lib/ens/AbstractENS.sol:7:5: Warning: Functions in interfaces should be declared external.
    function owner(bytes32 _node) public constant returns (address);
    ^--------------------------------------------------------------^
,@aragon/os/contracts/lib/ens/AbstractENS.sol:8:5: Warning: Functions in interfaces should be declared external.
    function resolver(bytes32 _node) public constant returns (address);
    ^-----------------------------------------------------------------^
,@aragon/os/contracts/lib/ens/AbstractENS.sol:9:5: Warning: Functions in interfaces should be declared external.
    function ttl(bytes32 _node) public constant returns (uint64);
    ^-----------------------------------------------------------^
,@aragon/os/contracts/lib/ens/AbstractENS.sol:10:5: Warning: Functions in interfaces should be declared external.
    function setOwner(bytes32 _node, address _owner) public;
    ^------------------------------------------------------^
,@aragon/os/contracts/lib/ens/AbstractENS.sol:11:5: Warning: Functions in interfaces should be declared external.
    function setSubnodeOwner(bytes32 _node, bytes32 label, address _owner) public;
    ^----------------------------------------------------------------------------^
,@aragon/os/contracts/lib/ens/AbstractENS.sol:12:5: Warning: Functions in interfaces should be declared external.
    function setResolver(bytes32 _node, address _resolver) public;
    ^------------------------------------------------------------^
,@aragon/os/contracts/lib/ens/AbstractENS.sol:13:5: Warning: Functions in interfaces should be declared external.
    function setTTL(bytes32 _node, uint64 _ttl) public;
    ^-------------------------------------------------^
,@aragon/os/contracts/lib/ens/ENS.sol:30:17: Warning: Decimal literal assigned to bytesXX variable will be left-aligned. Use an explicit conversion to silence this warning.
        records[0].owner = msg.sender;
                ^
,@aragon/os/contracts/lib/ens/ENS.sol:61:9: Warning: Invoking events without "emit" prefix is deprecated.
        Transfer(node, owner);
        ^-------------------^
,@aragon/os/contracts/lib/ens/ENS.sol:73:23: Warning: This function only accepts a single "bytes" argument. Please use "abi.encodePacked(...)" or a similar function to encode the data.
        var subnode = keccak256(node, label);
                      ^--------------------^
,@aragon/os/contracts/lib/ens/ENS.sol:74:9: Warning: Invoking events without "emit" prefix is deprecated.
        NewOwner(node, label, owner);
        ^--------------------------^
,@aragon/os/contracts/lib/ens/ENS.sol:84:9: Warning: Invoking events without "emit" prefix is deprecated.
        NewResolver(node, resolver);
        ^-------------------------^
,@aragon/os/contracts/lib/ens/ENS.sol:94:9: Warning: Invoking events without "emit" prefix is deprecated.
        NewTTL(node, ttl);
        ^---------------^
,@aragon/os/contracts/lib/ens/PublicResolver.sol:89:9: Warning: Invoking events without "emit" prefix is deprecated.
        AddrChanged(node, addr);
        ^---------------------^
,@aragon/os/contracts/lib/ens/PublicResolver.sol:113:9: Warning: Invoking events without "emit" prefix is deprecated.
        ContentChanged(node, hash);
        ^------------------------^
,@aragon/os/contracts/lib/ens/PublicResolver.sol:134:9: Warning: Invoking events without "emit" prefix is deprecated.
        NameChanged(node, name);
        ^---------------------^
,@aragon/os/contracts/lib/ens/PublicResolver.sol:169:9: Warning: Invoking events without "emit" prefix is deprecated.
        ABIChanged(node, contentType);
        ^---------------------------^
,@aragon/os/contracts/lib/ens/PublicResolver.sol:190:9: Warning: Invoking events without "emit" prefix is deprecated.
        PubkeyChanged(node, x, y);
        ^-----------------------^
,@aragon/os/contracts/lib/ens/PublicResolver.sol:212:9: Warning: Invoking events without "emit" prefix is deprecated.
        TextChanged(node, key, key);
        ^-------------------------^
,@aragon/id/contracts/ens/IPublicResolver.sol:5:5: Warning: Functions in interfaces should be declared external.
    function supportsInterface(bytes4 interfaceID) constant returns (bool);
    ^---------------------------------------------------------------------^
,@aragon/id/contracts/ens/IPublicResolver.sol:6:5: Warning: Functions in interfaces should be declared external.
    function addr(bytes32 node) constant returns (address ret);
    ^---------------------------------------------------------^
,@aragon/id/contracts/ens/IPublicResolver.sol:7:5: Warning: Functions in interfaces should be declared external.
    function setAddr(bytes32 node, address addr);
    ^-------------------------------------------^
,@aragon/id/contracts/ens/IPublicResolver.sol:8:5: Warning: Functions in interfaces should be declared external.
    function hash(bytes32 node) constant returns (bytes32 ret);
    ^---------------------------------------------------------^
,@aragon/id/contracts/ens/IPublicResolver.sol:9:5: Warning: Functions in interfaces should be declared external.
    function setHash(bytes32 node, bytes32 hash);
    ^-------------------------------------------^
,@aragon/id/contracts/IFIFSResolvingRegistrar.sol:8:5: Warning: Functions in interfaces should be declared external.
    function registerWithResolver(bytes32 _subnode, address _owner, IPublicResolver _resolver) public;
    ^------------------------------------------------------------------------------------------------^
,./templates/company-board/contracts/flat_CompanyBoardTemplate.sol:277:5: Warning: Functions in interfaces should be declared external.
    function hasPermission(address who, address where, bytes32 what, bytes how) public view returns (bool);
    ^-----------------------------------------------------------------------------------------------------^
,./templates/company-board/contracts/flat_CompanyBoardTemplate.sol:1044:5: Warning: Functions in interfaces should be declared external.
    function getScriptExecutor(bytes script) public view returns (IEVMScriptExecutor);
    ^--------------------------------------------------------------------------------^
,./templates/company-board/contracts/flat_CompanyBoardTemplate.sol:1404:5: Warning: Functions in interfaces should be declared external.
    function canForward(address sender, bytes evmCallScript) public view returns (bool);
    ^----------------------------------------------------------------------------------^
,./templates/company-board/contracts/flat_CompanyBoardTemplate.sol:1408:5: Warning: Functions in interfaces should be declared external.
    function forward(bytes evmCallScript) public;
    ^-------------------------------------------^
,./templates/company-board/contracts/flat_CompanyBoardTemplate.sol:1957:9: Warning: Invoking events without "emit" prefix is deprecated.
        Transfer(_from, _to, _amount);
        ^---------------------------^
,./templates/company-board/contracts/flat_CompanyBoardTemplate.sol:1989:9: Warning: Invoking events without "emit" prefix is deprecated.
        Approval(msg.sender, _spender, _amount);
        ^-------------------------------------^
,./templates/company-board/contracts/flat_CompanyBoardTemplate.sol:2117:9: Warning: Invoking events without "emit" prefix is deprecated.
        NewCloneToken(address(cloneToken), snapshot);
        ^------------------------------------------^
,./templates/company-board/contracts/flat_CompanyBoardTemplate.sol:2136:9: Warning: Invoking events without "emit" prefix is deprecated.
        Transfer(0, _owner, _amount);
        ^--------------------------^
,./templates/company-board/contracts/flat_CompanyBoardTemplate.sol:2152:9: Warning: Invoking events without "emit" prefix is deprecated.
        Transfer(_owner, 0, _amount);
        ^--------------------------^
,./templates/company-board/contracts/flat_CompanyBoardTemplate.sol:2253:33: Warning: Using contract member "balance" inherited from the address type is deprecated. Convert the contract to "address" type to access the member, for example use "address(contract).balance" instead.
            controller.transfer(this.balance);
                                ^----------^
,./templates/company-board/contracts/flat_CompanyBoardTemplate.sol:2260:9: Warning: Invoking events without "emit" prefix is deprecated.
        ClaimedTokens(_token, controller, balance);
        ^----------------------------------------^
,./templates/company-board/contracts/flat_CompanyBoardTemplate.sol:6315:5: Warning: Functions in interfaces should be declared external.
    function owner(bytes32 _node) public constant returns (address);
    ^--------------------------------------------------------------^
,./templates/company-board/contracts/flat_CompanyBoardTemplate.sol:6316:5: Warning: Functions in interfaces should be declared external.
    function resolver(bytes32 _node) public constant returns (address);
    ^-----------------------------------------------------------------^
,./templates/company-board/contracts/flat_CompanyBoardTemplate.sol:6317:5: Warning: Functions in interfaces should be declared external.
    function ttl(bytes32 _node) public constant returns (uint64);
    ^-----------------------------------------------------------^
,./templates/company-board/contracts/flat_CompanyBoardTemplate.sol:6318:5: Warning: Functions in interfaces should be declared external.
    function setOwner(bytes32 _node, address _owner) public;
    ^------------------------------------------------------^
,./templates/company-board/contracts/flat_CompanyBoardTemplate.sol:6319:5: Warning: Functions in interfaces should be declared external.
    function setSubnodeOwner(bytes32 _node, bytes32 label, address _owner) public;
    ^----------------------------------------------------------------------------^
,./templates/company-board/contracts/flat_CompanyBoardTemplate.sol:6320:5: Warning: Functions in interfaces should be declared external.
    function setResolver(bytes32 _node, address _resolver) public;
    ^------------------------------------------------------------^
,./templates/company-board/contracts/flat_CompanyBoardTemplate.sol:6321:5: Warning: Functions in interfaces should be declared external.
    function setTTL(bytes32 _node, uint64 _ttl) public;
    ^-------------------------------------------------^
,./templates/company-board/contracts/flat_CompanyBoardTemplate.sol:6365:17: Warning: Decimal literal assigned to bytesXX variable will be left-aligned. Use an explicit conversion to silence this warning.
        records[0].owner = msg.sender;
                ^
,./templates/company-board/contracts/flat_CompanyBoardTemplate.sol:6396:9: Warning: Invoking events without "emit" prefix is deprecated.
        Transfer(node, owner);
        ^-------------------^
,./templates/company-board/contracts/flat_CompanyBoardTemplate.sol:6408:23: Warning: This function only accepts a single "bytes" argument. Please use "abi.encodePacked(...)" or a similar function to encode the data.
        var subnode = keccak256(node, label);
                      ^--------------------^
,./templates/company-board/contracts/flat_CompanyBoardTemplate.sol:6409:9: Warning: Invoking events without "emit" prefix is deprecated.
        NewOwner(node, label, owner);
        ^--------------------------^
,./templates/company-board/contracts/flat_CompanyBoardTemplate.sol:6419:9: Warning: Invoking events without "emit" prefix is deprecated.
        NewResolver(node, resolver);
        ^-------------------------^
,./templates/company-board/contracts/flat_CompanyBoardTemplate.sol:6429:9: Warning: Invoking events without "emit" prefix is deprecated.
        NewTTL(node, ttl);
        ^---------------^
,./templates/company-board/contracts/flat_CompanyBoardTemplate.sol:6523:9: Warning: Invoking events without "emit" prefix is deprecated.
        AddrChanged(node, addr);
        ^---------------------^
,./templates/company-board/contracts/flat_CompanyBoardTemplate.sol:6547:9: Warning: Invoking events without "emit" prefix is deprecated.
        ContentChanged(node, hash);
        ^------------------------^
,./templates/company-board/contracts/flat_CompanyBoardTemplate.sol:6568:9: Warning: Invoking events without "emit" prefix is deprecated.
        NameChanged(node, name);
        ^---------------------^
,./templates/company-board/contracts/flat_CompanyBoardTemplate.sol:6603:9: Warning: Invoking events without "emit" prefix is deprecated.
        ABIChanged(node, contentType);
        ^---------------------------^
,./templates/company-board/contracts/flat_CompanyBoardTemplate.sol:6624:9: Warning: Invoking events without "emit" prefix is deprecated.
        PubkeyChanged(node, x, y);
        ^-----------------------^
,./templates/company-board/contracts/flat_CompanyBoardTemplate.sol:6646:9: Warning: Invoking events without "emit" prefix is deprecated.
        TextChanged(node, key, key);
        ^-------------------------^
,./templates/company-board/contracts/flat_CompanyBoardTemplate.sol:7101:5: Warning: Functions in interfaces should be declared external.
    function supportsInterface(bytes4 interfaceID) constant returns (bool);
    ^---------------------------------------------------------------------^
,./templates/company-board/contracts/flat_CompanyBoardTemplate.sol:7102:5: Warning: Functions in interfaces should be declared external.
    function addr(bytes32 node) constant returns (address ret);
    ^---------------------------------------------------------^
,./templates/company-board/contracts/flat_CompanyBoardTemplate.sol:7103:5: Warning: Functions in interfaces should be declared external.
    function setAddr(bytes32 node, address addr);
    ^-------------------------------------------^
,./templates/company-board/contracts/flat_CompanyBoardTemplate.sol:7104:5: Warning: Functions in interfaces should be declared external.
    function hash(bytes32 node) constant returns (bytes32 ret);
    ^---------------------------------------------------------^
,./templates/company-board/contracts/flat_CompanyBoardTemplate.sol:7105:5: Warning: Functions in interfaces should be declared external.
    function setHash(bytes32 node, bytes32 hash);
    ^-------------------------------------------^
,./templates/company-board/contracts/flat_CompanyBoardTemplate.sol:7116:5: Warning: Functions in interfaces should be declared external.
    function registerWithResolver(bytes32 _subnode, address _owner, IPublicResolver _resolver) public;
    ^------------------------------------------------------------------------------------------------^
,@aragon/id/contracts/FIFSResolvingRegistrar.sol:55:24: Warning: This function only accepts a single "bytes" argument. Please use "abi.encodePacked(...)" or a similar function to encode the data.
        bytes32 node = keccak256(rootNode, _subnode);
                       ^---------------------------^
,@aragon/os/contracts/common/VaultRecoverable.sol:49:34: Warning: Unused function parameter. Remove or comment out the variable name to silence this warning.
    function allowRecoverability(address token) public view returns (bool) {
                                 ^-----------^
,@aragon/id/contracts/ens/IPublicResolver.sol:5:5: Warning: No visibility specified. Defaulting to "public". In interfaces it defaults to external.
    function supportsInterface(bytes4 interfaceID) constant returns (bool);
    ^---------------------------------------------------------------------^
,@aragon/id/contracts/ens/IPublicResolver.sol:6:5: Warning: No visibility specified. Defaulting to "public". In interfaces it defaults to external.
    function addr(bytes32 node) constant returns (address ret);
    ^---------------------------------------------------------^
,@aragon/id/contracts/ens/IPublicResolver.sol:7:5: Warning: No visibility specified. Defaulting to "public". In interfaces it defaults to external.
    function setAddr(bytes32 node, address addr);
    ^-------------------------------------------^
,@aragon/id/contracts/ens/IPublicResolver.sol:8:5: Warning: No visibility specified. Defaulting to "public". In interfaces it defaults to external.
    function hash(bytes32 node) constant returns (bytes32 ret);
    ^---------------------------------------------------------^
,@aragon/id/contracts/ens/IPublicResolver.sol:9:5: Warning: No visibility specified. Defaulting to "public". In interfaces it defaults to external.
    function setHash(bytes32 node, bytes32 hash);
    ^-------------------------------------------^
,./templates/company-board/contracts/flat_CompanyBoardTemplate.sol:998:34: Warning: Unused function parameter. Remove or comment out the variable name to silence this warning.
    function allowRecoverability(address token) public view returns (bool) {
                                 ^-----------^
,./templates/company-board/contracts/flat_CompanyBoardTemplate.sol:7101:5: Warning: No visibility specified. Defaulting to "public". In interfaces it defaults to external.
    function supportsInterface(bytes4 interfaceID) constant returns (bool);
    ^---------------------------------------------------------------------^
,./templates/company-board/contracts/flat_CompanyBoardTemplate.sol:7102:5: Warning: No visibility specified. Defaulting to "public". In interfaces it defaults to external.
    function addr(bytes32 node) constant returns (address ret);
    ^---------------------------------------------------------^
,./templates/company-board/contracts/flat_CompanyBoardTemplate.sol:7103:5: Warning: No visibility specified. Defaulting to "public". In interfaces it defaults to external.
    function setAddr(bytes32 node, address addr);
    ^-------------------------------------------^
,./templates/company-board/contracts/flat_CompanyBoardTemplate.sol:7104:5: Warning: No visibility specified. Defaulting to "public". In interfaces it defaults to external.
    function hash(bytes32 node) constant returns (bytes32 ret);
    ^---------------------------------------------------------^
,./templates/company-board/contracts/flat_CompanyBoardTemplate.sol:7105:5: Warning: No visibility specified. Defaulting to "public". In interfaces it defaults to external.
    function setHash(bytes32 node, bytes32 hash);
    ^-------------------------------------------^
,./templates/company-board/contracts/flat_CompanyBoardTemplate.sol:3551:5: Warning: Function state mutability can be restricted to pure
    function getMaxPeriodTransitions() internal view returns (uint64) { return MAX_UINT64; }
    ^--------------------------------------------------------------------------------------^
,@aragon/apps-finance/contracts/Finance.sol:840:5: Warning: Function state mutability can be restricted to pure
    function getMaxPeriodTransitions() internal view returns (uint64) { return MAX_UINT64; }
    ^--------------------------------------------------------------------------------------^

Writing artifacts to ./build/contracts
```

## Membership

```console
$ npx truffle compile

Compiling ./contracts/MembershipTemplate.sol...
Compiling ./contracts/flat_MembershipTemplate.sol...
Compiling ./contracts/test/TestImports.sol...
Compiling @aragon/apps-agent/contracts/Agent.sol...
Compiling @aragon/apps-agent/contracts/SignatureValidator.sol...
Compiling @aragon/apps-agent/contracts/standards/ERC1271.sol...
Compiling @aragon/apps-agent/contracts/standards/IERC165.sol...
Compiling @aragon/apps-finance/contracts/Finance.sol...
Compiling @aragon/apps-payroll/contracts/Payroll.sol...
Compiling @aragon/apps-shared-minime/contracts/ITokenController.sol...
Compiling @aragon/apps-shared-minime/contracts/MiniMeToken.sol...
Compiling @aragon/apps-survey/contracts/Survey.sol...
Compiling @aragon/apps-token-manager/contracts/TokenManager.sol...
Compiling @aragon/apps-vault/contracts/Vault.sol...
Compiling @aragon/apps-voting/contracts/Voting.sol...
Compiling @aragon/id/contracts/FIFSResolvingRegistrar.sol...
Compiling @aragon/id/contracts/IFIFSResolvingRegistrar.sol...
Compiling @aragon/id/contracts/ens/IPublicResolver.sol...
Compiling @aragon/os/contracts/acl/ACL.sol...
Compiling @aragon/os/contracts/acl/ACLSyntaxSugar.sol...
Compiling @aragon/os/contracts/acl/IACL.sol...
Compiling @aragon/os/contracts/acl/IACLOracle.sol...
Compiling @aragon/os/contracts/apm/APMNamehash.sol...
Compiling @aragon/os/contracts/apm/APMRegistry.sol...
Compiling @aragon/os/contracts/apm/Repo.sol...
Compiling @aragon/os/contracts/apps/AppProxyBase.sol...
Compiling @aragon/os/contracts/apps/AppProxyPinned.sol...
Compiling @aragon/os/contracts/apps/AppProxyUpgradeable.sol...
Compiling @aragon/os/contracts/apps/AppStorage.sol...
Compiling @aragon/os/contracts/apps/AragonApp.sol...
Compiling @aragon/os/contracts/common/Autopetrified.sol...
Compiling @aragon/os/contracts/common/ConversionHelpers.sol...
Compiling @aragon/os/contracts/common/DelegateProxy.sol...
Compiling @aragon/os/contracts/common/DepositableDelegateProxy.sol...
Compiling @aragon/os/contracts/common/DepositableStorage.sol...
Compiling @aragon/os/contracts/common/EtherTokenConstant.sol...
Compiling @aragon/os/contracts/common/IForwarder.sol...
Compiling @aragon/os/contracts/common/IVaultRecoverable.sol...
Compiling @aragon/os/contracts/common/Initializable.sol...
Compiling @aragon/os/contracts/common/IsContract.sol...
Compiling @aragon/os/contracts/common/Petrifiable.sol...
Compiling @aragon/os/contracts/common/ReentrancyGuard.sol...
Compiling @aragon/os/contracts/common/SafeERC20.sol...
Compiling @aragon/os/contracts/common/TimeHelpers.sol...
Compiling @aragon/os/contracts/common/Uint256Helpers.sol...
Compiling @aragon/os/contracts/common/UnstructuredStorage.sol...
Compiling @aragon/os/contracts/common/VaultRecoverable.sol...
Compiling @aragon/os/contracts/ens/ENSConstants.sol...
Compiling @aragon/os/contracts/ens/ENSSubdomainRegistrar.sol...
Compiling @aragon/os/contracts/evmscript/EVMScriptRegistry.sol...
Compiling @aragon/os/contracts/evmscript/EVMScriptRunner.sol...
Compiling @aragon/os/contracts/evmscript/IEVMScriptExecutor.sol...
Compiling @aragon/os/contracts/evmscript/IEVMScriptRegistry.sol...
Compiling @aragon/os/contracts/evmscript/ScriptHelpers.sol...
Compiling @aragon/os/contracts/evmscript/executors/BaseEVMScriptExecutor.sol...
Compiling @aragon/os/contracts/evmscript/executors/CallsScript.sol...
Compiling @aragon/os/contracts/factory/APMRegistryFactory.sol...
Compiling @aragon/os/contracts/factory/AppProxyFactory.sol...
Compiling @aragon/os/contracts/factory/DAOFactory.sol...
Compiling @aragon/os/contracts/factory/ENSFactory.sol...
Compiling @aragon/os/contracts/factory/EVMScriptRegistryFactory.sol...
Compiling @aragon/os/contracts/kernel/IKernel.sol...
Compiling @aragon/os/contracts/kernel/Kernel.sol...
Compiling @aragon/os/contracts/kernel/KernelConstants.sol...
Compiling @aragon/os/contracts/kernel/KernelProxy.sol...
Compiling @aragon/os/contracts/kernel/KernelStorage.sol...
Compiling @aragon/os/contracts/lib/ens/AbstractENS.sol...
Compiling @aragon/os/contracts/lib/ens/ENS.sol...
Compiling @aragon/os/contracts/lib/ens/PublicResolver.sol...
Compiling @aragon/os/contracts/lib/math/SafeMath.sol...
Compiling @aragon/os/contracts/lib/math/SafeMath64.sol...
Compiling @aragon/os/contracts/lib/misc/ERCProxy.sol...
Compiling @aragon/os/contracts/lib/token/ERC20.sol...
Compiling @aragon/ppf-contracts/contracts/IFeed.sol...
Compiling @aragon/templates-shared/contracts/BaseTemplate.sol...
Compiling @aragon/templates-shared/contracts/Migrations.sol...
Compiling @aragon/templates-shared/contracts/TokenCache.sol...
Compiling @aragon/templates-shared/contracts/test/mocks/ExecutionTarget.sol...

Compilation warnings encountered:

@aragon/apps-shared-minime/contracts/MiniMeToken.sol:37:5: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
    function Controlled()  public { controller = msg.sender;}
    ^-------------------------------------------------------^
,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:123:5: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
    function MiniMeToken(
    ^ (Relevant source part starts here and spans across multiple lines).
,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:195:9: Warning: Use of the "var" keyword is deprecated.
        var previousBalanceFrom = balanceOfAt(_from, block.number);
        ^---------------------^
,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:209:9: Warning: Use of the "var" keyword is deprecated.
        var previousBalanceTo = balanceOfAt(_to, block.number);
        ^-------------------^
,@aragon/os/contracts/lib/ens/ENS.sol:22:48: Warning: "throw" is deprecated in favour of "revert()", "require()" and "assert()".
        if (records[node].owner != msg.sender) throw;
                                               ^---^
,@aragon/os/contracts/lib/ens/ENS.sol:29:5: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
    function ENS() public {
    ^ (Relevant source part starts here and spans across multiple lines).
,@aragon/os/contracts/lib/ens/ENS.sol:73:9: Warning: Use of the "var" keyword is deprecated.
        var subnode = keccak256(node, label);
        ^---------^
,@aragon/os/contracts/lib/ens/PublicResolver.sol:45:44: Warning: "throw" is deprecated in favour of "revert()", "require()" and "assert()".
        if (ens.owner(node) != msg.sender) throw;
                                           ^---^
,@aragon/os/contracts/lib/ens/PublicResolver.sol:53:5: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
    function PublicResolver(AbstractENS ensAddr) public {
    ^ (Relevant source part starts here and spans across multiple lines).
,@aragon/os/contracts/lib/ens/PublicResolver.sol:146:9: Warning: Use of the "var" keyword is deprecated.
        var record = records[node];
        ^--------^
,@aragon/os/contracts/lib/ens/PublicResolver.sol:166:53: Warning: "throw" is deprecated in favour of "revert()", "require()" and "assert()".
        if (((contentType - 1) & contentType) != 0) throw;
                                                    ^---^
,./templates/membership/contracts/flat_MembershipTemplate.sol:69:5: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
    function Controlled()  public { controller = msg.sender;}
    ^-------------------------------------------------------^
,./templates/membership/contracts/flat_MembershipTemplate.sol:155:5: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
    function MiniMeToken(
    ^ (Relevant source part starts here and spans across multiple lines).
,./templates/membership/contracts/flat_MembershipTemplate.sol:227:9: Warning: Use of the "var" keyword is deprecated.
        var previousBalanceFrom = balanceOfAt(_from, block.number);
        ^---------------------^
,./templates/membership/contracts/flat_MembershipTemplate.sol:241:9: Warning: Use of the "var" keyword is deprecated.
        var previousBalanceTo = balanceOfAt(_to, block.number);
        ^-------------------^
,./templates/membership/contracts/flat_MembershipTemplate.sol:6381:48: Warning: "throw" is deprecated in favour of "revert()", "require()" and "assert()".
        if (records[node].owner != msg.sender) throw;
                                               ^---^
,./templates/membership/contracts/flat_MembershipTemplate.sol:6388:5: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
    function ENS() public {
    ^ (Relevant source part starts here and spans across multiple lines).
,./templates/membership/contracts/flat_MembershipTemplate.sol:6432:9: Warning: Use of the "var" keyword is deprecated.
        var subnode = keccak256(node, label);
        ^---------^
,./templates/membership/contracts/flat_MembershipTemplate.sol:6503:44: Warning: "throw" is deprecated in favour of "revert()", "require()" and "assert()".
        if (ens.owner(node) != msg.sender) throw;
                                           ^---^
,./templates/membership/contracts/flat_MembershipTemplate.sol:6511:5: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
    function PublicResolver(AbstractENS ensAddr) public {
    ^ (Relevant source part starts here and spans across multiple lines).
,./templates/membership/contracts/flat_MembershipTemplate.sol:6604:9: Warning: Use of the "var" keyword is deprecated.
        var record = records[node];
        ^--------^
,./templates/membership/contracts/flat_MembershipTemplate.sol:6624:53: Warning: "throw" is deprecated in favour of "revert()", "require()" and "assert()".
        if (((contentType - 1) & contentType) != 0) throw;
                                                    ^---^
,@aragon/templates-shared/contracts/Migrations.sol:11:3: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
  function Migrations() public {
  ^ (Relevant source part starts here and spans across multiple lines).
,@aragon/os/contracts/lib/ens/ENS.sol:60:37: Warning: This declaration shadows an existing declaration.
    function setOwner(bytes32 node, address owner) only_owner(node) public {
                                    ^-----------^
@aragon/os/contracts/lib/ens/ENS.sol:36:5: The shadowed declaration is here:
    function owner(bytes32 node) public constant returns (address) {
    ^ (Relevant source part starts here and spans across multiple lines).

,@aragon/os/contracts/lib/ens/ENS.sol:72:59: Warning: This declaration shadows an existing declaration.
    function setSubnodeOwner(bytes32 node, bytes32 label, address owner) only_owner(node) public {
                                                          ^-----------^
@aragon/os/contracts/lib/ens/ENS.sol:36:5: The shadowed declaration is here:
    function owner(bytes32 node) public constant returns (address) {
    ^ (Relevant source part starts here and spans across multiple lines).

,@aragon/os/contracts/lib/ens/ENS.sol:83:40: Warning: This declaration shadows an existing declaration.
    function setResolver(bytes32 node, address resolver) only_owner(node) public {
                                       ^--------------^
@aragon/os/contracts/lib/ens/ENS.sol:43:5: The shadowed declaration is here:
    function resolver(bytes32 node) public constant returns (address) {
    ^ (Relevant source part starts here and spans across multiple lines).

,@aragon/os/contracts/lib/ens/ENS.sol:93:35: Warning: This declaration shadows an existing declaration.
    function setTTL(bytes32 node, uint64 ttl) only_owner(node) public {
                                  ^--------^
@aragon/os/contracts/lib/ens/ENS.sol:50:5: The shadowed declaration is here:
    function ttl(bytes32 node) public constant returns (uint64) {
    ^ (Relevant source part starts here and spans across multiple lines).

,@aragon/os/contracts/lib/ens/PublicResolver.sol:87:36: Warning: This declaration shadows an existing declaration.
    function setAddr(bytes32 node, address addr) only_owner(node) public {
                                   ^----------^
@aragon/os/contracts/lib/ens/PublicResolver.sol:77:5: The shadowed declaration is here:
    function addr(bytes32 node) public constant returns (address ret) {
    ^ (Relevant source part starts here and spans across multiple lines).

,@aragon/os/contracts/lib/ens/PublicResolver.sol:132:36: Warning: This declaration shadows an existing declaration.
    function setName(bytes32 node, string name) only_owner(node) public {
                                   ^---------^
@aragon/os/contracts/lib/ens/PublicResolver.sol:122:5: The shadowed declaration is here:
    function name(bytes32 node) public constant returns (string ret) {
    ^ (Relevant source part starts here and spans across multiple lines).

,@aragon/id/contracts/ens/IPublicResolver.sol:7:36: Warning: This declaration shadows an existing declaration.
    function setAddr(bytes32 node, address addr);
                                   ^----------^
@aragon/id/contracts/ens/IPublicResolver.sol:6:5: The shadowed declaration is here:
    function addr(bytes32 node) constant returns (address ret);
    ^---------------------------------------------------------^

,@aragon/id/contracts/ens/IPublicResolver.sol:9:36: Warning: This declaration shadows an existing declaration.
    function setHash(bytes32 node, bytes32 hash);
                                   ^----------^
@aragon/id/contracts/ens/IPublicResolver.sol:8:5: The shadowed declaration is here:
    function hash(bytes32 node) constant returns (bytes32 ret);
    ^---------------------------------------------------------^

,./templates/membership/contracts/flat_MembershipTemplate.sol:6419:37: Warning: This declaration shadows an existing declaration.
    function setOwner(bytes32 node, address owner) only_owner(node) public {
                                    ^-----------^
./templates/membership/contracts/flat_MembershipTemplate.sol:6395:5: The shadowed declaration is here:
    function owner(bytes32 node) public constant returns (address) {
    ^ (Relevant source part starts here and spans across multiple lines).

,./templates/membership/contracts/flat_MembershipTemplate.sol:6431:59: Warning: This declaration shadows an existing declaration.
    function setSubnodeOwner(bytes32 node, bytes32 label, address owner) only_owner(node) public {
                                                          ^-----------^
./templates/membership/contracts/flat_MembershipTemplate.sol:6395:5: The shadowed declaration is here:
    function owner(bytes32 node) public constant returns (address) {
    ^ (Relevant source part starts here and spans across multiple lines).

,./templates/membership/contracts/flat_MembershipTemplate.sol:6442:40: Warning: This declaration shadows an existing declaration.
    function setResolver(bytes32 node, address resolver) only_owner(node) public {
                                       ^--------------^
./templates/membership/contracts/flat_MembershipTemplate.sol:6402:5: The shadowed declaration is here:
    function resolver(bytes32 node) public constant returns (address) {
    ^ (Relevant source part starts here and spans across multiple lines).

,./templates/membership/contracts/flat_MembershipTemplate.sol:6452:35: Warning: This declaration shadows an existing declaration.
    function setTTL(bytes32 node, uint64 ttl) only_owner(node) public {
                                  ^--------^
./templates/membership/contracts/flat_MembershipTemplate.sol:6409:5: The shadowed declaration is here:
    function ttl(bytes32 node) public constant returns (uint64) {
    ^ (Relevant source part starts here and spans across multiple lines).

,./templates/membership/contracts/flat_MembershipTemplate.sol:6545:36: Warning: This declaration shadows an existing declaration.
    function setAddr(bytes32 node, address addr) only_owner(node) public {
                                   ^----------^
./templates/membership/contracts/flat_MembershipTemplate.sol:6535:5: The shadowed declaration is here:
    function addr(bytes32 node) public constant returns (address ret) {
    ^ (Relevant source part starts here and spans across multiple lines).

,./templates/membership/contracts/flat_MembershipTemplate.sol:6590:36: Warning: This declaration shadows an existing declaration.
    function setName(bytes32 node, string name) only_owner(node) public {
                                   ^---------^
./templates/membership/contracts/flat_MembershipTemplate.sol:6580:5: The shadowed declaration is here:
    function name(bytes32 node) public constant returns (string ret) {
    ^ (Relevant source part starts here and spans across multiple lines).

,./templates/membership/contracts/flat_MembershipTemplate.sol:7127:36: Warning: This declaration shadows an existing declaration.
    function setAddr(bytes32 node, address addr);
                                   ^----------^
./templates/membership/contracts/flat_MembershipTemplate.sol:7126:5: The shadowed declaration is here:
    function addr(bytes32 node) constant returns (address ret);
    ^---------------------------------------------------------^

,./templates/membership/contracts/flat_MembershipTemplate.sol:7129:36: Warning: This declaration shadows an existing declaration.
    function setHash(bytes32 node, bytes32 hash);
                                   ^----------^
./templates/membership/contracts/flat_MembershipTemplate.sol:7128:5: The shadowed declaration is here:
    function hash(bytes32 node) constant returns (bytes32 ret);
    ^---------------------------------------------------------^

,@aragon/apps-vault/contracts/Vault.sol:76:5: Warning: Variable is shadowed in inline assembly by an instruction of the same name
    function balance(address _token) public view returns (uint256) {
    ^ (Relevant source part starts here and spans across multiple lines).
,@aragon/apps-vault/contracts/Vault.sol:76:5: Warning: Variable is shadowed in inline assembly by an instruction of the same name
    function balance(address _token) public view returns (uint256) {
    ^ (Relevant source part starts here and spans across multiple lines).
,./templates/membership/contracts/flat_MembershipTemplate.sol:1987:5: Warning: Variable is shadowed in inline assembly by an instruction of the same name
    function balance(address _token) public view returns (uint256) {
    ^ (Relevant source part starts here and spans across multiple lines).
,./templates/membership/contracts/flat_MembershipTemplate.sol:1987:5: Warning: Variable is shadowed in inline assembly by an instruction of the same name
    function balance(address _token) public view returns (uint256) {
    ^ (Relevant source part starts here and spans across multiple lines).
,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:213:9: Warning: Invoking events without "emit" prefix is deprecated.
        Transfer(_from, _to, _amount);
        ^---------------------------^
,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:245:9: Warning: Invoking events without "emit" prefix is deprecated.
        Approval(msg.sender, _spender, _amount);
        ^-------------------------------------^
,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:373:9: Warning: Invoking events without "emit" prefix is deprecated.
        NewCloneToken(address(cloneToken), snapshot);
        ^------------------------------------------^
,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:392:9: Warning: Invoking events without "emit" prefix is deprecated.
        Transfer(0, _owner, _amount);
        ^--------------------------^
,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:408:9: Warning: Invoking events without "emit" prefix is deprecated.
        Transfer(_owner, 0, _amount);
        ^--------------------------^
,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:509:33: Warning: Using contract member "balance" inherited from the address type is deprecated. Convert the contract to "address" type to access the member, for example use "address(contract).balance" instead.
            controller.transfer(this.balance);
                                ^----------^
,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:516:9: Warning: Invoking events without "emit" prefix is deprecated.
        ClaimedTokens(_token, controller, balance);
        ^----------------------------------------^
,@aragon/os/contracts/acl/IACL.sol:13:5: Warning: Functions in interfaces should be declared external.
    function hasPermission(address who, address where, bytes32 what, bytes how) public view returns (bool);
    ^-----------------------------------------------------------------------------------------------------^
,@aragon/os/contracts/evmscript/IEVMScriptRegistry.sol:24:5: Warning: Functions in interfaces should be declared external.
    function getScriptExecutor(bytes script) public view returns (IEVMScriptExecutor);
    ^--------------------------------------------------------------------------------^
,@aragon/os/contracts/common/IForwarder.sol:13:5: Warning: Functions in interfaces should be declared external.
    function canForward(address sender, bytes evmCallScript) public view returns (bool);
    ^----------------------------------------------------------------------------------^
,@aragon/os/contracts/common/IForwarder.sol:17:5: Warning: Functions in interfaces should be declared external.
    function forward(bytes evmCallScript) public;
    ^-------------------------------------------^
,@aragon/os/contracts/lib/ens/AbstractENS.sol:7:5: Warning: Functions in interfaces should be declared external.
    function owner(bytes32 _node) public constant returns (address);
    ^--------------------------------------------------------------^
,@aragon/os/contracts/lib/ens/AbstractENS.sol:8:5: Warning: Functions in interfaces should be declared external.
    function resolver(bytes32 _node) public constant returns (address);
    ^-----------------------------------------------------------------^
,@aragon/os/contracts/lib/ens/AbstractENS.sol:9:5: Warning: Functions in interfaces should be declared external.
    function ttl(bytes32 _node) public constant returns (uint64);
    ^-----------------------------------------------------------^
,@aragon/os/contracts/lib/ens/AbstractENS.sol:10:5: Warning: Functions in interfaces should be declared external.
    function setOwner(bytes32 _node, address _owner) public;
    ^------------------------------------------------------^
,@aragon/os/contracts/lib/ens/AbstractENS.sol:11:5: Warning: Functions in interfaces should be declared external.
    function setSubnodeOwner(bytes32 _node, bytes32 label, address _owner) public;
    ^----------------------------------------------------------------------------^
,@aragon/os/contracts/lib/ens/AbstractENS.sol:12:5: Warning: Functions in interfaces should be declared external.
    function setResolver(bytes32 _node, address _resolver) public;
    ^------------------------------------------------------------^
,@aragon/os/contracts/lib/ens/AbstractENS.sol:13:5: Warning: Functions in interfaces should be declared external.
    function setTTL(bytes32 _node, uint64 _ttl) public;
    ^-------------------------------------------------^
,@aragon/os/contracts/lib/ens/ENS.sol:30:17: Warning: Decimal literal assigned to bytesXX variable will be left-aligned. Use an explicit conversion to silence this warning.
        records[0].owner = msg.sender;
                ^
,@aragon/os/contracts/lib/ens/ENS.sol:61:9: Warning: Invoking events without "emit" prefix is deprecated.
        Transfer(node, owner);
        ^-------------------^
,@aragon/os/contracts/lib/ens/ENS.sol:73:23: Warning: This function only accepts a single "bytes" argument. Please use "abi.encodePacked(...)" or a similar function to encode the data.
        var subnode = keccak256(node, label);
                      ^--------------------^
,@aragon/os/contracts/lib/ens/ENS.sol:74:9: Warning: Invoking events without "emit" prefix is deprecated.
        NewOwner(node, label, owner);
        ^--------------------------^
,@aragon/os/contracts/lib/ens/ENS.sol:84:9: Warning: Invoking events without "emit" prefix is deprecated.
        NewResolver(node, resolver);
        ^-------------------------^
,@aragon/os/contracts/lib/ens/ENS.sol:94:9: Warning: Invoking events without "emit" prefix is deprecated.
        NewTTL(node, ttl);
        ^---------------^
,@aragon/os/contracts/lib/ens/PublicResolver.sol:89:9: Warning: Invoking events without "emit" prefix is deprecated.
        AddrChanged(node, addr);
        ^---------------------^
,@aragon/os/contracts/lib/ens/PublicResolver.sol:113:9: Warning: Invoking events without "emit" prefix is deprecated.
        ContentChanged(node, hash);
        ^------------------------^
,@aragon/os/contracts/lib/ens/PublicResolver.sol:134:9: Warning: Invoking events without "emit" prefix is deprecated.
        NameChanged(node, name);
        ^---------------------^
,@aragon/os/contracts/lib/ens/PublicResolver.sol:169:9: Warning: Invoking events without "emit" prefix is deprecated.
        ABIChanged(node, contentType);
        ^---------------------------^
,@aragon/os/contracts/lib/ens/PublicResolver.sol:190:9: Warning: Invoking events without "emit" prefix is deprecated.
        PubkeyChanged(node, x, y);
        ^-----------------------^
,@aragon/os/contracts/lib/ens/PublicResolver.sol:212:9: Warning: Invoking events without "emit" prefix is deprecated.
        TextChanged(node, key, key);
        ^-------------------------^
,@aragon/id/contracts/ens/IPublicResolver.sol:5:5: Warning: Functions in interfaces should be declared external.
    function supportsInterface(bytes4 interfaceID) constant returns (bool);
    ^---------------------------------------------------------------------^
,@aragon/id/contracts/ens/IPublicResolver.sol:6:5: Warning: Functions in interfaces should be declared external.
    function addr(bytes32 node) constant returns (address ret);
    ^---------------------------------------------------------^
,@aragon/id/contracts/ens/IPublicResolver.sol:7:5: Warning: Functions in interfaces should be declared external.
    function setAddr(bytes32 node, address addr);
    ^-------------------------------------------^
,@aragon/id/contracts/ens/IPublicResolver.sol:8:5: Warning: Functions in interfaces should be declared external.
    function hash(bytes32 node) constant returns (bytes32 ret);
    ^---------------------------------------------------------^
,@aragon/id/contracts/ens/IPublicResolver.sol:9:5: Warning: Functions in interfaces should be declared external.
    function setHash(bytes32 node, bytes32 hash);
    ^-------------------------------------------^
,@aragon/id/contracts/IFIFSResolvingRegistrar.sol:8:5: Warning: Functions in interfaces should be declared external.
    function registerWithResolver(bytes32 _subnode, address _owner, IPublicResolver _resolver) public;
    ^------------------------------------------------------------------------------------------------^
,./templates/membership/contracts/flat_MembershipTemplate.sol:245:9: Warning: Invoking events without "emit" prefix is deprecated.
        Transfer(_from, _to, _amount);
        ^---------------------------^
,./templates/membership/contracts/flat_MembershipTemplate.sol:277:9: Warning: Invoking events without "emit" prefix is deprecated.
        Approval(msg.sender, _spender, _amount);
        ^-------------------------------------^
,./templates/membership/contracts/flat_MembershipTemplate.sol:405:9: Warning: Invoking events without "emit" prefix is deprecated.
        NewCloneToken(address(cloneToken), snapshot);
        ^------------------------------------------^
,./templates/membership/contracts/flat_MembershipTemplate.sol:424:9: Warning: Invoking events without "emit" prefix is deprecated.
        Transfer(0, _owner, _amount);
        ^--------------------------^
,./templates/membership/contracts/flat_MembershipTemplate.sol:440:9: Warning: Invoking events without "emit" prefix is deprecated.
        Transfer(_owner, 0, _amount);
        ^--------------------------^
,./templates/membership/contracts/flat_MembershipTemplate.sol:541:33: Warning: Using contract member "balance" inherited from the address type is deprecated. Convert the contract to "address" type to access the member, for example use "address(contract).balance" instead.
            controller.transfer(this.balance);
                                ^----------^
,./templates/membership/contracts/flat_MembershipTemplate.sol:548:9: Warning: Invoking events without "emit" prefix is deprecated.
        ClaimedTokens(_token, controller, balance);
        ^----------------------------------------^
,./templates/membership/contracts/flat_MembershipTemplate.sol:908:5: Warning: Functions in interfaces should be declared external.
    function hasPermission(address who, address where, bytes32 what, bytes how) public view returns (bool);
    ^-----------------------------------------------------------------------------------------------------^
,./templates/membership/contracts/flat_MembershipTemplate.sol:1675:5: Warning: Functions in interfaces should be declared external.
    function getScriptExecutor(bytes script) public view returns (IEVMScriptExecutor);
    ^--------------------------------------------------------------------------------^
,./templates/membership/contracts/flat_MembershipTemplate.sol:2035:5: Warning: Functions in interfaces should be declared external.
    function canForward(address sender, bytes evmCallScript) public view returns (bool);
    ^----------------------------------------------------------------------------------^
,./templates/membership/contracts/flat_MembershipTemplate.sol:2039:5: Warning: Functions in interfaces should be declared external.
    function forward(bytes evmCallScript) public;
    ^-------------------------------------------^
,./templates/membership/contracts/flat_MembershipTemplate.sol:6339:5: Warning: Functions in interfaces should be declared external.
    function owner(bytes32 _node) public constant returns (address);
    ^--------------------------------------------------------------^
,./templates/membership/contracts/flat_MembershipTemplate.sol:6340:5: Warning: Functions in interfaces should be declared external.
    function resolver(bytes32 _node) public constant returns (address);
    ^-----------------------------------------------------------------^
,./templates/membership/contracts/flat_MembershipTemplate.sol:6341:5: Warning: Functions in interfaces should be declared external.
    function ttl(bytes32 _node) public constant returns (uint64);
    ^-----------------------------------------------------------^
,./templates/membership/contracts/flat_MembershipTemplate.sol:6342:5: Warning: Functions in interfaces should be declared external.
    function setOwner(bytes32 _node, address _owner) public;
    ^------------------------------------------------------^
,./templates/membership/contracts/flat_MembershipTemplate.sol:6343:5: Warning: Functions in interfaces should be declared external.
    function setSubnodeOwner(bytes32 _node, bytes32 label, address _owner) public;
    ^----------------------------------------------------------------------------^
,./templates/membership/contracts/flat_MembershipTemplate.sol:6344:5: Warning: Functions in interfaces should be declared external.
    function setResolver(bytes32 _node, address _resolver) public;
    ^------------------------------------------------------------^
,./templates/membership/contracts/flat_MembershipTemplate.sol:6345:5: Warning: Functions in interfaces should be declared external.
    function setTTL(bytes32 _node, uint64 _ttl) public;
    ^-------------------------------------------------^
,./templates/membership/contracts/flat_MembershipTemplate.sol:6389:17: Warning: Decimal literal assigned to bytesXX variable will be left-aligned. Use an explicit conversion to silence this warning.
        records[0].owner = msg.sender;
                ^
,./templates/membership/contracts/flat_MembershipTemplate.sol:6420:9: Warning: Invoking events without "emit" prefix is deprecated.
        Transfer(node, owner);
        ^-------------------^
,./templates/membership/contracts/flat_MembershipTemplate.sol:6432:23: Warning: This function only accepts a single "bytes" argument. Please use "abi.encodePacked(...)" or a similar function to encode the data.
        var subnode = keccak256(node, label);
                      ^--------------------^
,./templates/membership/contracts/flat_MembershipTemplate.sol:6433:9: Warning: Invoking events without "emit" prefix is deprecated.
        NewOwner(node, label, owner);
        ^--------------------------^
,./templates/membership/contracts/flat_MembershipTemplate.sol:6443:9: Warning: Invoking events without "emit" prefix is deprecated.
        NewResolver(node, resolver);
        ^-------------------------^
,./templates/membership/contracts/flat_MembershipTemplate.sol:6453:9: Warning: Invoking events without "emit" prefix is deprecated.
        NewTTL(node, ttl);
        ^---------------^
,./templates/membership/contracts/flat_MembershipTemplate.sol:6547:9: Warning: Invoking events without "emit" prefix is deprecated.
        AddrChanged(node, addr);
        ^---------------------^
,./templates/membership/contracts/flat_MembershipTemplate.sol:6571:9: Warning: Invoking events without "emit" prefix is deprecated.
        ContentChanged(node, hash);
        ^------------------------^
,./templates/membership/contracts/flat_MembershipTemplate.sol:6592:9: Warning: Invoking events without "emit" prefix is deprecated.
        NameChanged(node, name);
        ^---------------------^
,./templates/membership/contracts/flat_MembershipTemplate.sol:6627:9: Warning: Invoking events without "emit" prefix is deprecated.
        ABIChanged(node, contentType);
        ^---------------------------^
,./templates/membership/contracts/flat_MembershipTemplate.sol:6648:9: Warning: Invoking events without "emit" prefix is deprecated.
        PubkeyChanged(node, x, y);
        ^-----------------------^
,./templates/membership/contracts/flat_MembershipTemplate.sol:6670:9: Warning: Invoking events without "emit" prefix is deprecated.
        TextChanged(node, key, key);
        ^-------------------------^
,./templates/membership/contracts/flat_MembershipTemplate.sol:7125:5: Warning: Functions in interfaces should be declared external.
    function supportsInterface(bytes4 interfaceID) constant returns (bool);
    ^---------------------------------------------------------------------^
,./templates/membership/contracts/flat_MembershipTemplate.sol:7126:5: Warning: Functions in interfaces should be declared external.
    function addr(bytes32 node) constant returns (address ret);
    ^---------------------------------------------------------^
,./templates/membership/contracts/flat_MembershipTemplate.sol:7127:5: Warning: Functions in interfaces should be declared external.
    function setAddr(bytes32 node, address addr);
    ^-------------------------------------------^
,./templates/membership/contracts/flat_MembershipTemplate.sol:7128:5: Warning: Functions in interfaces should be declared external.
    function hash(bytes32 node) constant returns (bytes32 ret);
    ^---------------------------------------------------------^
,./templates/membership/contracts/flat_MembershipTemplate.sol:7129:5: Warning: Functions in interfaces should be declared external.
    function setHash(bytes32 node, bytes32 hash);
    ^-------------------------------------------^
,./templates/membership/contracts/flat_MembershipTemplate.sol:7140:5: Warning: Functions in interfaces should be declared external.
    function registerWithResolver(bytes32 _subnode, address _owner, IPublicResolver _resolver) public;
    ^------------------------------------------------------------------------------------------------^
,@aragon/id/contracts/FIFSResolvingRegistrar.sol:55:24: Warning: This function only accepts a single "bytes" argument. Please use "abi.encodePacked(...)" or a similar function to encode the data.
        bytes32 node = keccak256(rootNode, _subnode);
                       ^---------------------------^
,@aragon/os/contracts/common/VaultRecoverable.sol:49:34: Warning: Unused function parameter. Remove or comment out the variable name to silence this warning.
    function allowRecoverability(address token) public view returns (bool) {
                                 ^-----------^
,@aragon/id/contracts/ens/IPublicResolver.sol:5:5: Warning: No visibility specified. Defaulting to "public". In interfaces it defaults to external.
    function supportsInterface(bytes4 interfaceID) constant returns (bool);
    ^---------------------------------------------------------------------^
,@aragon/id/contracts/ens/IPublicResolver.sol:6:5: Warning: No visibility specified. Defaulting to "public". In interfaces it defaults to external.
    function addr(bytes32 node) constant returns (address ret);
    ^---------------------------------------------------------^
,@aragon/id/contracts/ens/IPublicResolver.sol:7:5: Warning: No visibility specified. Defaulting to "public". In interfaces it defaults to external.
    function setAddr(bytes32 node, address addr);
    ^-------------------------------------------^
,@aragon/id/contracts/ens/IPublicResolver.sol:8:5: Warning: No visibility specified. Defaulting to "public". In interfaces it defaults to external.
    function hash(bytes32 node) constant returns (bytes32 ret);
    ^---------------------------------------------------------^
,@aragon/id/contracts/ens/IPublicResolver.sol:9:5: Warning: No visibility specified. Defaulting to "public". In interfaces it defaults to external.
    function setHash(bytes32 node, bytes32 hash);
    ^-------------------------------------------^
,./templates/membership/contracts/flat_MembershipTemplate.sol:1629:34: Warning: Unused function parameter. Remove or comment out the variable name to silence this warning.
    function allowRecoverability(address token) public view returns (bool) {
                                 ^-----------^
,./templates/membership/contracts/flat_MembershipTemplate.sol:7125:5: Warning: No visibility specified. Defaulting to "public". In interfaces it defaults to external.
    function supportsInterface(bytes4 interfaceID) constant returns (bool);
    ^---------------------------------------------------------------------^
,./templates/membership/contracts/flat_MembershipTemplate.sol:7126:5: Warning: No visibility specified. Defaulting to "public". In interfaces it defaults to external.
    function addr(bytes32 node) constant returns (address ret);
    ^---------------------------------------------------------^
,./templates/membership/contracts/flat_MembershipTemplate.sol:7127:5: Warning: No visibility specified. Defaulting to "public". In interfaces it defaults to external.
    function setAddr(bytes32 node, address addr);
    ^-------------------------------------------^
,./templates/membership/contracts/flat_MembershipTemplate.sol:7128:5: Warning: No visibility specified. Defaulting to "public". In interfaces it defaults to external.
    function hash(bytes32 node) constant returns (bytes32 ret);
    ^---------------------------------------------------------^
,./templates/membership/contracts/flat_MembershipTemplate.sol:7129:5: Warning: No visibility specified. Defaulting to "public". In interfaces it defaults to external.
    function setHash(bytes32 node, bytes32 hash);
    ^-------------------------------------------^
,./templates/membership/contracts/flat_MembershipTemplate.sol:3575:5: Warning: Function state mutability can be restricted to pure
    function getMaxPeriodTransitions() internal view returns (uint64) { return MAX_UINT64; }
    ^--------------------------------------------------------------------------------------^
,@aragon/apps-finance/contracts/Finance.sol:840:5: Warning: Function state mutability can be restricted to pure
    function getMaxPeriodTransitions() internal view returns (uint64) { return MAX_UINT64; }
    ^--------------------------------------------------------------------------------------^

Writing artifacts to ./build/contracts
```

## Reputation

```console
$ npx truffle compile

Compiling ./contracts/ReputationTemplate.sol...
Compiling ./contracts/flat_ReputationTemplate.sol...
Compiling ./contracts/test/TestImports.sol...
Compiling @aragon/apps-agent/contracts/Agent.sol...
Compiling @aragon/apps-agent/contracts/SignatureValidator.sol...
Compiling @aragon/apps-agent/contracts/standards/ERC1271.sol...
Compiling @aragon/apps-agent/contracts/standards/IERC165.sol...
Compiling @aragon/apps-finance/contracts/Finance.sol...
Compiling @aragon/apps-payroll/contracts/Payroll.sol...
Compiling @aragon/apps-shared-minime/contracts/ITokenController.sol...
Compiling @aragon/apps-shared-minime/contracts/MiniMeToken.sol...
Compiling @aragon/apps-survey/contracts/Survey.sol...
Compiling @aragon/apps-token-manager/contracts/TokenManager.sol...
Compiling @aragon/apps-vault/contracts/Vault.sol...
Compiling @aragon/apps-voting/contracts/Voting.sol...
Compiling @aragon/id/contracts/FIFSResolvingRegistrar.sol...
Compiling @aragon/id/contracts/IFIFSResolvingRegistrar.sol...
Compiling @aragon/id/contracts/ens/IPublicResolver.sol...
Compiling @aragon/os/contracts/acl/ACL.sol...
Compiling @aragon/os/contracts/acl/ACLSyntaxSugar.sol...
Compiling @aragon/os/contracts/acl/IACL.sol...
Compiling @aragon/os/contracts/acl/IACLOracle.sol...
Compiling @aragon/os/contracts/apm/APMNamehash.sol...
Compiling @aragon/os/contracts/apm/APMRegistry.sol...
Compiling @aragon/os/contracts/apm/Repo.sol...
Compiling @aragon/os/contracts/apps/AppProxyBase.sol...
Compiling @aragon/os/contracts/apps/AppProxyPinned.sol...
Compiling @aragon/os/contracts/apps/AppProxyUpgradeable.sol...
Compiling @aragon/os/contracts/apps/AppStorage.sol...
Compiling @aragon/os/contracts/apps/AragonApp.sol...
Compiling @aragon/os/contracts/common/Autopetrified.sol...
Compiling @aragon/os/contracts/common/ConversionHelpers.sol...
Compiling @aragon/os/contracts/common/DelegateProxy.sol...
Compiling @aragon/os/contracts/common/DepositableDelegateProxy.sol...
Compiling @aragon/os/contracts/common/DepositableStorage.sol...
Compiling @aragon/os/contracts/common/EtherTokenConstant.sol...
Compiling @aragon/os/contracts/common/IForwarder.sol...
Compiling @aragon/os/contracts/common/IVaultRecoverable.sol...
Compiling @aragon/os/contracts/common/Initializable.sol...
Compiling @aragon/os/contracts/common/IsContract.sol...
Compiling @aragon/os/contracts/common/Petrifiable.sol...
Compiling @aragon/os/contracts/common/ReentrancyGuard.sol...
Compiling @aragon/os/contracts/common/SafeERC20.sol...
Compiling @aragon/os/contracts/common/TimeHelpers.sol...
Compiling @aragon/os/contracts/common/Uint256Helpers.sol...
Compiling @aragon/os/contracts/common/UnstructuredStorage.sol...
Compiling @aragon/os/contracts/common/VaultRecoverable.sol...
Compiling @aragon/os/contracts/ens/ENSConstants.sol...
Compiling @aragon/os/contracts/ens/ENSSubdomainRegistrar.sol...
Compiling @aragon/os/contracts/evmscript/EVMScriptRegistry.sol...
Compiling @aragon/os/contracts/evmscript/EVMScriptRunner.sol...
Compiling @aragon/os/contracts/evmscript/IEVMScriptExecutor.sol...
Compiling @aragon/os/contracts/evmscript/IEVMScriptRegistry.sol...
Compiling @aragon/os/contracts/evmscript/ScriptHelpers.sol...
Compiling @aragon/os/contracts/evmscript/executors/BaseEVMScriptExecutor.sol...
Compiling @aragon/os/contracts/evmscript/executors/CallsScript.sol...
Compiling @aragon/os/contracts/factory/APMRegistryFactory.sol...
Compiling @aragon/os/contracts/factory/AppProxyFactory.sol...
Compiling @aragon/os/contracts/factory/DAOFactory.sol...
Compiling @aragon/os/contracts/factory/ENSFactory.sol...
Compiling @aragon/os/contracts/factory/EVMScriptRegistryFactory.sol...
Compiling @aragon/os/contracts/kernel/IKernel.sol...
Compiling @aragon/os/contracts/kernel/Kernel.sol...
Compiling @aragon/os/contracts/kernel/KernelConstants.sol...
Compiling @aragon/os/contracts/kernel/KernelProxy.sol...
Compiling @aragon/os/contracts/kernel/KernelStorage.sol...
Compiling @aragon/os/contracts/lib/ens/AbstractENS.sol...
Compiling @aragon/os/contracts/lib/ens/ENS.sol...
Compiling @aragon/os/contracts/lib/ens/PublicResolver.sol...
Compiling @aragon/os/contracts/lib/math/SafeMath.sol...
Compiling @aragon/os/contracts/lib/math/SafeMath64.sol...
Compiling @aragon/os/contracts/lib/misc/ERCProxy.sol...
Compiling @aragon/os/contracts/lib/token/ERC20.sol...
Compiling @aragon/ppf-contracts/contracts/IFeed.sol...
Compiling @aragon/templates-shared/contracts/BaseTemplate.sol...
Compiling @aragon/templates-shared/contracts/Migrations.sol...
Compiling @aragon/templates-shared/contracts/TokenCache.sol...
Compiling @aragon/templates-shared/contracts/test/mocks/ExecutionTarget.sol...

Compilation warnings encountered:

@aragon/apps-shared-minime/contracts/MiniMeToken.sol:37:5: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
    function Controlled()  public { controller = msg.sender;}
    ^-------------------------------------------------------^
,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:123:5: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
    function MiniMeToken(
    ^ (Relevant source part starts here and spans across multiple lines).
,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:195:9: Warning: Use of the "var" keyword is deprecated.
        var previousBalanceFrom = balanceOfAt(_from, block.number);
        ^---------------------^
,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:209:9: Warning: Use of the "var" keyword is deprecated.
        var previousBalanceTo = balanceOfAt(_to, block.number);
        ^-------------------^
,@aragon/os/contracts/lib/ens/ENS.sol:22:48: Warning: "throw" is deprecated in favour of "revert()", "require()" and "assert()".
        if (records[node].owner != msg.sender) throw;
                                               ^---^
,@aragon/os/contracts/lib/ens/ENS.sol:29:5: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
    function ENS() public {
    ^ (Relevant source part starts here and spans across multiple lines).
,@aragon/os/contracts/lib/ens/ENS.sol:73:9: Warning: Use of the "var" keyword is deprecated.
        var subnode = keccak256(node, label);
        ^---------^
,@aragon/os/contracts/lib/ens/PublicResolver.sol:45:44: Warning: "throw" is deprecated in favour of "revert()", "require()" and "assert()".
        if (ens.owner(node) != msg.sender) throw;
                                           ^---^
,@aragon/os/contracts/lib/ens/PublicResolver.sol:53:5: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
    function PublicResolver(AbstractENS ensAddr) public {
    ^ (Relevant source part starts here and spans across multiple lines).
,@aragon/os/contracts/lib/ens/PublicResolver.sol:146:9: Warning: Use of the "var" keyword is deprecated.
        var record = records[node];
        ^--------^
,@aragon/os/contracts/lib/ens/PublicResolver.sol:166:53: Warning: "throw" is deprecated in favour of "revert()", "require()" and "assert()".
        if (((contentType - 1) & contentType) != 0) throw;
                                                    ^---^
,./templates/reputation/contracts/flat_ReputationTemplate.sol:69:5: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
    function Controlled()  public { controller = msg.sender;}
    ^-------------------------------------------------------^
,./templates/reputation/contracts/flat_ReputationTemplate.sol:155:5: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
    function MiniMeToken(
    ^ (Relevant source part starts here and spans across multiple lines).
,./templates/reputation/contracts/flat_ReputationTemplate.sol:227:9: Warning: Use of the "var" keyword is deprecated.
        var previousBalanceFrom = balanceOfAt(_from, block.number);
        ^---------------------^
,./templates/reputation/contracts/flat_ReputationTemplate.sol:241:9: Warning: Use of the "var" keyword is deprecated.
        var previousBalanceTo = balanceOfAt(_to, block.number);
        ^-------------------^
,./templates/reputation/contracts/flat_ReputationTemplate.sol:6381:48: Warning: "throw" is deprecated in favour of "revert()", "require()" and "assert()".
        if (records[node].owner != msg.sender) throw;
                                               ^---^
,./templates/reputation/contracts/flat_ReputationTemplate.sol:6388:5: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
    function ENS() public {
    ^ (Relevant source part starts here and spans across multiple lines).
,./templates/reputation/contracts/flat_ReputationTemplate.sol:6432:9: Warning: Use of the "var" keyword is deprecated.
        var subnode = keccak256(node, label);
        ^---------^
,./templates/reputation/contracts/flat_ReputationTemplate.sol:6503:44: Warning: "throw" is deprecated in favour of "revert()", "require()" and "assert()".
        if (ens.owner(node) != msg.sender) throw;
                                           ^---^
,./templates/reputation/contracts/flat_ReputationTemplate.sol:6511:5: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
    function PublicResolver(AbstractENS ensAddr) public {
    ^ (Relevant source part starts here and spans across multiple lines).
,./templates/reputation/contracts/flat_ReputationTemplate.sol:6604:9: Warning: Use of the "var" keyword is deprecated.
        var record = records[node];
        ^--------^
,./templates/reputation/contracts/flat_ReputationTemplate.sol:6624:53: Warning: "throw" is deprecated in favour of "revert()", "require()" and "assert()".
        if (((contentType - 1) & contentType) != 0) throw;
                                                    ^---^
,@aragon/templates-shared/contracts/Migrations.sol:11:3: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
  function Migrations() public {
  ^ (Relevant source part starts here and spans across multiple lines).
,@aragon/os/contracts/lib/ens/ENS.sol:60:37: Warning: This declaration shadows an existing declaration.
    function setOwner(bytes32 node, address owner) only_owner(node) public {
                                    ^-----------^
@aragon/os/contracts/lib/ens/ENS.sol:36:5: The shadowed declaration is here:
    function owner(bytes32 node) public constant returns (address) {
    ^ (Relevant source part starts here and spans across multiple lines).

,@aragon/os/contracts/lib/ens/ENS.sol:72:59: Warning: This declaration shadows an existing declaration.
    function setSubnodeOwner(bytes32 node, bytes32 label, address owner) only_owner(node) public {
                                                          ^-----------^
@aragon/os/contracts/lib/ens/ENS.sol:36:5: The shadowed declaration is here:
    function owner(bytes32 node) public constant returns (address) {
    ^ (Relevant source part starts here and spans across multiple lines).

,@aragon/os/contracts/lib/ens/ENS.sol:83:40: Warning: This declaration shadows an existing declaration.
    function setResolver(bytes32 node, address resolver) only_owner(node) public {
                                       ^--------------^
@aragon/os/contracts/lib/ens/ENS.sol:43:5: The shadowed declaration is here:
    function resolver(bytes32 node) public constant returns (address) {
    ^ (Relevant source part starts here and spans across multiple lines).

,@aragon/os/contracts/lib/ens/ENS.sol:93:35: Warning: This declaration shadows an existing declaration.
    function setTTL(bytes32 node, uint64 ttl) only_owner(node) public {
                                  ^--------^
@aragon/os/contracts/lib/ens/ENS.sol:50:5: The shadowed declaration is here:
    function ttl(bytes32 node) public constant returns (uint64) {
    ^ (Relevant source part starts here and spans across multiple lines).

,@aragon/os/contracts/lib/ens/PublicResolver.sol:87:36: Warning: This declaration shadows an existing declaration.
    function setAddr(bytes32 node, address addr) only_owner(node) public {
                                   ^----------^
@aragon/os/contracts/lib/ens/PublicResolver.sol:77:5: The shadowed declaration is here:
    function addr(bytes32 node) public constant returns (address ret) {
    ^ (Relevant source part starts here and spans across multiple lines).

,@aragon/os/contracts/lib/ens/PublicResolver.sol:132:36: Warning: This declaration shadows an existing declaration.
    function setName(bytes32 node, string name) only_owner(node) public {
                                   ^---------^
@aragon/os/contracts/lib/ens/PublicResolver.sol:122:5: The shadowed declaration is here:
    function name(bytes32 node) public constant returns (string ret) {
    ^ (Relevant source part starts here and spans across multiple lines).

,@aragon/id/contracts/ens/IPublicResolver.sol:7:36: Warning: This declaration shadows an existing declaration.
    function setAddr(bytes32 node, address addr);
                                   ^----------^
@aragon/id/contracts/ens/IPublicResolver.sol:6:5: The shadowed declaration is here:
    function addr(bytes32 node) constant returns (address ret);
    ^---------------------------------------------------------^

,@aragon/id/contracts/ens/IPublicResolver.sol:9:36: Warning: This declaration shadows an existing declaration.
    function setHash(bytes32 node, bytes32 hash);
                                   ^----------^
@aragon/id/contracts/ens/IPublicResolver.sol:8:5: The shadowed declaration is here:
    function hash(bytes32 node) constant returns (bytes32 ret);
    ^---------------------------------------------------------^

,./templates/reputation/contracts/flat_ReputationTemplate.sol:6419:37: Warning: This declaration shadows an existing declaration.
    function setOwner(bytes32 node, address owner) only_owner(node) public {
                                    ^-----------^
./templates/reputation/contracts/flat_ReputationTemplate.sol:6395:5: The shadowed declaration is here:
    function owner(bytes32 node) public constant returns (address) {
    ^ (Relevant source part starts here and spans across multiple lines).

,./templates/reputation/contracts/flat_ReputationTemplate.sol:6431:59: Warning: This declaration shadows an existing declaration.
    function setSubnodeOwner(bytes32 node, bytes32 label, address owner) only_owner(node) public {
                                                          ^-----------^
./templates/reputation/contracts/flat_ReputationTemplate.sol:6395:5: The shadowed declaration is here:
    function owner(bytes32 node) public constant returns (address) {
    ^ (Relevant source part starts here and spans across multiple lines).

,./templates/reputation/contracts/flat_ReputationTemplate.sol:6442:40: Warning: This declaration shadows an existing declaration.
    function setResolver(bytes32 node, address resolver) only_owner(node) public {
                                       ^--------------^
./templates/reputation/contracts/flat_ReputationTemplate.sol:6402:5: The shadowed declaration is here:
    function resolver(bytes32 node) public constant returns (address) {
    ^ (Relevant source part starts here and spans across multiple lines).

,./templates/reputation/contracts/flat_ReputationTemplate.sol:6452:35: Warning: This declaration shadows an existing declaration.
    function setTTL(bytes32 node, uint64 ttl) only_owner(node) public {
                                  ^--------^
./templates/reputation/contracts/flat_ReputationTemplate.sol:6409:5: The shadowed declaration is here:
    function ttl(bytes32 node) public constant returns (uint64) {
    ^ (Relevant source part starts here and spans across multiple lines).

,./templates/reputation/contracts/flat_ReputationTemplate.sol:6545:36: Warning: This declaration shadows an existing declaration.
    function setAddr(bytes32 node, address addr) only_owner(node) public {
                                   ^----------^
./templates/reputation/contracts/flat_ReputationTemplate.sol:6535:5: The shadowed declaration is here:
    function addr(bytes32 node) public constant returns (address ret) {
    ^ (Relevant source part starts here and spans across multiple lines).

,./templates/reputation/contracts/flat_ReputationTemplate.sol:6590:36: Warning: This declaration shadows an existing declaration.
    function setName(bytes32 node, string name) only_owner(node) public {
                                   ^---------^
./templates/reputation/contracts/flat_ReputationTemplate.sol:6580:5: The shadowed declaration is here:
    function name(bytes32 node) public constant returns (string ret) {
    ^ (Relevant source part starts here and spans across multiple lines).

,./templates/reputation/contracts/flat_ReputationTemplate.sol:7127:36: Warning: This declaration shadows an existing declaration.
    function setAddr(bytes32 node, address addr);
                                   ^----------^
./templates/reputation/contracts/flat_ReputationTemplate.sol:7126:5: The shadowed declaration is here:
    function addr(bytes32 node) constant returns (address ret);
    ^---------------------------------------------------------^

,./templates/reputation/contracts/flat_ReputationTemplate.sol:7129:36: Warning: This declaration shadows an existing declaration.
    function setHash(bytes32 node, bytes32 hash);
                                   ^----------^
./templates/reputation/contracts/flat_ReputationTemplate.sol:7128:5: The shadowed declaration is here:
    function hash(bytes32 node) constant returns (bytes32 ret);
    ^---------------------------------------------------------^

,@aragon/apps-vault/contracts/Vault.sol:76:5: Warning: Variable is shadowed in inline assembly by an instruction of the same name
    function balance(address _token) public view returns (uint256) {
    ^ (Relevant source part starts here and spans across multiple lines).
,@aragon/apps-vault/contracts/Vault.sol:76:5: Warning: Variable is shadowed in inline assembly by an instruction of the same name
    function balance(address _token) public view returns (uint256) {
    ^ (Relevant source part starts here and spans across multiple lines).
,./templates/reputation/contracts/flat_ReputationTemplate.sol:1987:5: Warning: Variable is shadowed in inline assembly by an instruction of the same name
    function balance(address _token) public view returns (uint256) {
    ^ (Relevant source part starts here and spans across multiple lines).
,./templates/reputation/contracts/flat_ReputationTemplate.sol:1987:5: Warning: Variable is shadowed in inline assembly by an instruction of the same name
    function balance(address _token) public view returns (uint256) {
    ^ (Relevant source part starts here and spans across multiple lines).
,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:213:9: Warning: Invoking events without "emit" prefix is deprecated.
        Transfer(_from, _to, _amount);
        ^---------------------------^
,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:245:9: Warning: Invoking events without "emit" prefix is deprecated.
        Approval(msg.sender, _spender, _amount);
        ^-------------------------------------^
,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:373:9: Warning: Invoking events without "emit" prefix is deprecated.
        NewCloneToken(address(cloneToken), snapshot);
        ^------------------------------------------^
,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:392:9: Warning: Invoking events without "emit" prefix is deprecated.
        Transfer(0, _owner, _amount);
        ^--------------------------^
,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:408:9: Warning: Invoking events without "emit" prefix is deprecated.
        Transfer(_owner, 0, _amount);
        ^--------------------------^
,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:509:33: Warning: Using contract member "balance" inherited from the address type is deprecated. Convert the contract to "address" type to access the member, for example use "address(contract).balance" instead.
            controller.transfer(this.balance);
                                ^----------^
,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:516:9: Warning: Invoking events without "emit" prefix is deprecated.
        ClaimedTokens(_token, controller, balance);
        ^----------------------------------------^
,@aragon/os/contracts/acl/IACL.sol:13:5: Warning: Functions in interfaces should be declared external.
    function hasPermission(address who, address where, bytes32 what, bytes how) public view returns (bool);
    ^-----------------------------------------------------------------------------------------------------^
,@aragon/os/contracts/evmscript/IEVMScriptRegistry.sol:24:5: Warning: Functions in interfaces should be declared external.
    function getScriptExecutor(bytes script) public view returns (IEVMScriptExecutor);
    ^--------------------------------------------------------------------------------^
,@aragon/os/contracts/common/IForwarder.sol:13:5: Warning: Functions in interfaces should be declared external.
    function canForward(address sender, bytes evmCallScript) public view returns (bool);
    ^----------------------------------------------------------------------------------^
,@aragon/os/contracts/common/IForwarder.sol:17:5: Warning: Functions in interfaces should be declared external.
    function forward(bytes evmCallScript) public;
    ^-------------------------------------------^
,@aragon/os/contracts/lib/ens/AbstractENS.sol:7:5: Warning: Functions in interfaces should be declared external.
    function owner(bytes32 _node) public constant returns (address);
    ^--------------------------------------------------------------^
,@aragon/os/contracts/lib/ens/AbstractENS.sol:8:5: Warning: Functions in interfaces should be declared external.
    function resolver(bytes32 _node) public constant returns (address);
    ^-----------------------------------------------------------------^
,@aragon/os/contracts/lib/ens/AbstractENS.sol:9:5: Warning: Functions in interfaces should be declared external.
    function ttl(bytes32 _node) public constant returns (uint64);
    ^-----------------------------------------------------------^
,@aragon/os/contracts/lib/ens/AbstractENS.sol:10:5: Warning: Functions in interfaces should be declared external.
    function setOwner(bytes32 _node, address _owner) public;
    ^------------------------------------------------------^
,@aragon/os/contracts/lib/ens/AbstractENS.sol:11:5: Warning: Functions in interfaces should be declared external.
    function setSubnodeOwner(bytes32 _node, bytes32 label, address _owner) public;
    ^----------------------------------------------------------------------------^
,@aragon/os/contracts/lib/ens/AbstractENS.sol:12:5: Warning: Functions in interfaces should be declared external.
    function setResolver(bytes32 _node, address _resolver) public;
    ^------------------------------------------------------------^
,@aragon/os/contracts/lib/ens/AbstractENS.sol:13:5: Warning: Functions in interfaces should be declared external.
    function setTTL(bytes32 _node, uint64 _ttl) public;
    ^-------------------------------------------------^
,@aragon/os/contracts/lib/ens/ENS.sol:30:17: Warning: Decimal literal assigned to bytesXX variable will be left-aligned. Use an explicit conversion to silence this warning.
        records[0].owner = msg.sender;
                ^
,@aragon/os/contracts/lib/ens/ENS.sol:61:9: Warning: Invoking events without "emit" prefix is deprecated.
        Transfer(node, owner);
        ^-------------------^
,@aragon/os/contracts/lib/ens/ENS.sol:73:23: Warning: This function only accepts a single "bytes" argument. Please use "abi.encodePacked(...)" or a similar function to encode the data.
        var subnode = keccak256(node, label);
                      ^--------------------^
,@aragon/os/contracts/lib/ens/ENS.sol:74:9: Warning: Invoking events without "emit" prefix is deprecated.
        NewOwner(node, label, owner);
        ^--------------------------^
,@aragon/os/contracts/lib/ens/ENS.sol:84:9: Warning: Invoking events without "emit" prefix is deprecated.
        NewResolver(node, resolver);
        ^-------------------------^
,@aragon/os/contracts/lib/ens/ENS.sol:94:9: Warning: Invoking events without "emit" prefix is deprecated.
        NewTTL(node, ttl);
        ^---------------^
,@aragon/os/contracts/lib/ens/PublicResolver.sol:89:9: Warning: Invoking events without "emit" prefix is deprecated.
        AddrChanged(node, addr);
        ^---------------------^
,@aragon/os/contracts/lib/ens/PublicResolver.sol:113:9: Warning: Invoking events without "emit" prefix is deprecated.
        ContentChanged(node, hash);
        ^------------------------^
,@aragon/os/contracts/lib/ens/PublicResolver.sol:134:9: Warning: Invoking events without "emit" prefix is deprecated.
        NameChanged(node, name);
        ^---------------------^
,@aragon/os/contracts/lib/ens/PublicResolver.sol:169:9: Warning: Invoking events without "emit" prefix is deprecated.
        ABIChanged(node, contentType);
        ^---------------------------^
,@aragon/os/contracts/lib/ens/PublicResolver.sol:190:9: Warning: Invoking events without "emit" prefix is deprecated.
        PubkeyChanged(node, x, y);
        ^-----------------------^
,@aragon/os/contracts/lib/ens/PublicResolver.sol:212:9: Warning: Invoking events without "emit" prefix is deprecated.
        TextChanged(node, key, key);
        ^-------------------------^
,@aragon/id/contracts/ens/IPublicResolver.sol:5:5: Warning: Functions in interfaces should be declared external.
    function supportsInterface(bytes4 interfaceID) constant returns (bool);
    ^---------------------------------------------------------------------^
,@aragon/id/contracts/ens/IPublicResolver.sol:6:5: Warning: Functions in interfaces should be declared external.
    function addr(bytes32 node) constant returns (address ret);
    ^---------------------------------------------------------^
,@aragon/id/contracts/ens/IPublicResolver.sol:7:5: Warning: Functions in interfaces should be declared external.
    function setAddr(bytes32 node, address addr);
    ^-------------------------------------------^
,@aragon/id/contracts/ens/IPublicResolver.sol:8:5: Warning: Functions in interfaces should be declared external.
    function hash(bytes32 node) constant returns (bytes32 ret);
    ^---------------------------------------------------------^
,@aragon/id/contracts/ens/IPublicResolver.sol:9:5: Warning: Functions in interfaces should be declared external.
    function setHash(bytes32 node, bytes32 hash);
    ^-------------------------------------------^
,@aragon/id/contracts/IFIFSResolvingRegistrar.sol:8:5: Warning: Functions in interfaces should be declared external.
    function registerWithResolver(bytes32 _subnode, address _owner, IPublicResolver _resolver) public;
    ^------------------------------------------------------------------------------------------------^
,./templates/reputation/contracts/flat_ReputationTemplate.sol:245:9: Warning: Invoking events without "emit" prefix is deprecated.
        Transfer(_from, _to, _amount);
        ^---------------------------^
,./templates/reputation/contracts/flat_ReputationTemplate.sol:277:9: Warning: Invoking events without "emit" prefix is deprecated.
        Approval(msg.sender, _spender, _amount);
        ^-------------------------------------^
,./templates/reputation/contracts/flat_ReputationTemplate.sol:405:9: Warning: Invoking events without "emit" prefix is deprecated.
        NewCloneToken(address(cloneToken), snapshot);
        ^------------------------------------------^
,./templates/reputation/contracts/flat_ReputationTemplate.sol:424:9: Warning: Invoking events without "emit" prefix is deprecated.
        Transfer(0, _owner, _amount);
        ^--------------------------^
,./templates/reputation/contracts/flat_ReputationTemplate.sol:440:9: Warning: Invoking events without "emit" prefix is deprecated.
        Transfer(_owner, 0, _amount);
        ^--------------------------^
,./templates/reputation/contracts/flat_ReputationTemplate.sol:541:33: Warning: Using contract member "balance" inherited from the address type is deprecated. Convert the contract to "address" type to access the member, for example use "address(contract).balance" instead.
            controller.transfer(this.balance);
                                ^----------^
,./templates/reputation/contracts/flat_ReputationTemplate.sol:548:9: Warning: Invoking events without "emit" prefix is deprecated.
        ClaimedTokens(_token, controller, balance);
        ^----------------------------------------^
,./templates/reputation/contracts/flat_ReputationTemplate.sol:908:5: Warning: Functions in interfaces should be declared external.
    function hasPermission(address who, address where, bytes32 what, bytes how) public view returns (bool);
    ^-----------------------------------------------------------------------------------------------------^
,./templates/reputation/contracts/flat_ReputationTemplate.sol:1675:5: Warning: Functions in interfaces should be declared external.
    function getScriptExecutor(bytes script) public view returns (IEVMScriptExecutor);
    ^--------------------------------------------------------------------------------^
,./templates/reputation/contracts/flat_ReputationTemplate.sol:2035:5: Warning: Functions in interfaces should be declared external.
    function canForward(address sender, bytes evmCallScript) public view returns (bool);
    ^----------------------------------------------------------------------------------^
,./templates/reputation/contracts/flat_ReputationTemplate.sol:2039:5: Warning: Functions in interfaces should be declared external.
    function forward(bytes evmCallScript) public;
    ^-------------------------------------------^
,./templates/reputation/contracts/flat_ReputationTemplate.sol:6339:5: Warning: Functions in interfaces should be declared external.
    function owner(bytes32 _node) public constant returns (address);
    ^--------------------------------------------------------------^
,./templates/reputation/contracts/flat_ReputationTemplate.sol:6340:5: Warning: Functions in interfaces should be declared external.
    function resolver(bytes32 _node) public constant returns (address);
    ^-----------------------------------------------------------------^
,./templates/reputation/contracts/flat_ReputationTemplate.sol:6341:5: Warning: Functions in interfaces should be declared external.
    function ttl(bytes32 _node) public constant returns (uint64);
    ^-----------------------------------------------------------^
,./templates/reputation/contracts/flat_ReputationTemplate.sol:6342:5: Warning: Functions in interfaces should be declared external.
    function setOwner(bytes32 _node, address _owner) public;
    ^------------------------------------------------------^
,./templates/reputation/contracts/flat_ReputationTemplate.sol:6343:5: Warning: Functions in interfaces should be declared external.
    function setSubnodeOwner(bytes32 _node, bytes32 label, address _owner) public;
    ^----------------------------------------------------------------------------^
,./templates/reputation/contracts/flat_ReputationTemplate.sol:6344:5: Warning: Functions in interfaces should be declared external.
    function setResolver(bytes32 _node, address _resolver) public;
    ^------------------------------------------------------------^
,./templates/reputation/contracts/flat_ReputationTemplate.sol:6345:5: Warning: Functions in interfaces should be declared external.
    function setTTL(bytes32 _node, uint64 _ttl) public;
    ^-------------------------------------------------^
,./templates/reputation/contracts/flat_ReputationTemplate.sol:6389:17: Warning: Decimal literal assigned to bytesXX variable will be left-aligned. Use an explicit conversion to silence this warning.
        records[0].owner = msg.sender;
                ^
,./templates/reputation/contracts/flat_ReputationTemplate.sol:6420:9: Warning: Invoking events without "emit" prefix is deprecated.
        Transfer(node, owner);
        ^-------------------^
,./templates/reputation/contracts/flat_ReputationTemplate.sol:6432:23: Warning: This function only accepts a single "bytes" argument. Please use "abi.encodePacked(...)" or a similar function to encode the data.
        var subnode = keccak256(node, label);
                      ^--------------------^
,./templates/reputation/contracts/flat_ReputationTemplate.sol:6433:9: Warning: Invoking events without "emit" prefix is deprecated.
        NewOwner(node, label, owner);
        ^--------------------------^
,./templates/reputation/contracts/flat_ReputationTemplate.sol:6443:9: Warning: Invoking events without "emit" prefix is deprecated.
        NewResolver(node, resolver);
        ^-------------------------^
,./templates/reputation/contracts/flat_ReputationTemplate.sol:6453:9: Warning: Invoking events without "emit" prefix is deprecated.
        NewTTL(node, ttl);
        ^---------------^
,./templates/reputation/contracts/flat_ReputationTemplate.sol:6547:9: Warning: Invoking events without "emit" prefix is deprecated.
        AddrChanged(node, addr);
        ^---------------------^
,./templates/reputation/contracts/flat_ReputationTemplate.sol:6571:9: Warning: Invoking events without "emit" prefix is deprecated.
        ContentChanged(node, hash);
        ^------------------------^
,./templates/reputation/contracts/flat_ReputationTemplate.sol:6592:9: Warning: Invoking events without "emit" prefix is deprecated.
        NameChanged(node, name);
        ^---------------------^
,./templates/reputation/contracts/flat_ReputationTemplate.sol:6627:9: Warning: Invoking events without "emit" prefix is deprecated.
        ABIChanged(node, contentType);
        ^---------------------------^
,./templates/reputation/contracts/flat_ReputationTemplate.sol:6648:9: Warning: Invoking events without "emit" prefix is deprecated.
        PubkeyChanged(node, x, y);
        ^-----------------------^
,./templates/reputation/contracts/flat_ReputationTemplate.sol:6670:9: Warning: Invoking events without "emit" prefix is deprecated.
        TextChanged(node, key, key);
        ^-------------------------^
,./templates/reputation/contracts/flat_ReputationTemplate.sol:7125:5: Warning: Functions in interfaces should be declared external.
    function supportsInterface(bytes4 interfaceID) constant returns (bool);
    ^---------------------------------------------------------------------^
,./templates/reputation/contracts/flat_ReputationTemplate.sol:7126:5: Warning: Functions in interfaces should be declared external.
    function addr(bytes32 node) constant returns (address ret);
    ^---------------------------------------------------------^
,./templates/reputation/contracts/flat_ReputationTemplate.sol:7127:5: Warning: Functions in interfaces should be declared external.
    function setAddr(bytes32 node, address addr);
    ^-------------------------------------------^
,./templates/reputation/contracts/flat_ReputationTemplate.sol:7128:5: Warning: Functions in interfaces should be declared external.
    function hash(bytes32 node) constant returns (bytes32 ret);
    ^---------------------------------------------------------^
,./templates/reputation/contracts/flat_ReputationTemplate.sol:7129:5: Warning: Functions in interfaces should be declared external.
    function setHash(bytes32 node, bytes32 hash);
    ^-------------------------------------------^
,./templates/reputation/contracts/flat_ReputationTemplate.sol:7140:5: Warning: Functions in interfaces should be declared external.
    function registerWithResolver(bytes32 _subnode, address _owner, IPublicResolver _resolver) public;
    ^------------------------------------------------------------------------------------------------^
,@aragon/id/contracts/FIFSResolvingRegistrar.sol:55:24: Warning: This function only accepts a single "bytes" argument. Please use "abi.encodePacked(...)" or a similar function to encode the data.
        bytes32 node = keccak256(rootNode, _subnode);
                       ^---------------------------^
,@aragon/os/contracts/common/VaultRecoverable.sol:49:34: Warning: Unused function parameter. Remove or comment out the variable name to silence this warning.
    function allowRecoverability(address token) public view returns (bool) {
                                 ^-----------^
,@aragon/id/contracts/ens/IPublicResolver.sol:5:5: Warning: No visibility specified. Defaulting to "public". In interfaces it defaults to external.
    function supportsInterface(bytes4 interfaceID) constant returns (bool);
    ^---------------------------------------------------------------------^
,@aragon/id/contracts/ens/IPublicResolver.sol:6:5: Warning: No visibility specified. Defaulting to "public". In interfaces it defaults to external.
    function addr(bytes32 node) constant returns (address ret);
    ^---------------------------------------------------------^
,@aragon/id/contracts/ens/IPublicResolver.sol:7:5: Warning: No visibility specified. Defaulting to "public". In interfaces it defaults to external.
    function setAddr(bytes32 node, address addr);
    ^-------------------------------------------^
,@aragon/id/contracts/ens/IPublicResolver.sol:8:5: Warning: No visibility specified. Defaulting to "public". In interfaces it defaults to external.
    function hash(bytes32 node) constant returns (bytes32 ret);
    ^---------------------------------------------------------^
,@aragon/id/contracts/ens/IPublicResolver.sol:9:5: Warning: No visibility specified. Defaulting to "public". In interfaces it defaults to external.
    function setHash(bytes32 node, bytes32 hash);
    ^-------------------------------------------^
,./templates/reputation/contracts/flat_ReputationTemplate.sol:1629:34: Warning: Unused function parameter. Remove or comment out the variable name to silence this warning.
    function allowRecoverability(address token) public view returns (bool) {
                                 ^-----------^
,./templates/reputation/contracts/flat_ReputationTemplate.sol:7125:5: Warning: No visibility specified. Defaulting to "public". In interfaces it defaults to external.
    function supportsInterface(bytes4 interfaceID) constant returns (bool);
    ^---------------------------------------------------------------------^
,./templates/reputation/contracts/flat_ReputationTemplate.sol:7126:5: Warning: No visibility specified. Defaulting to "public". In interfaces it defaults to external.
    function addr(bytes32 node) constant returns (address ret);
    ^---------------------------------------------------------^
,./templates/reputation/contracts/flat_ReputationTemplate.sol:7127:5: Warning: No visibility specified. Defaulting to "public". In interfaces it defaults to external.
    function setAddr(bytes32 node, address addr);
    ^-------------------------------------------^
,./templates/reputation/contracts/flat_ReputationTemplate.sol:7128:5: Warning: No visibility specified. Defaulting to "public". In interfaces it defaults to external.
    function hash(bytes32 node) constant returns (bytes32 ret);
    ^---------------------------------------------------------^
,./templates/reputation/contracts/flat_ReputationTemplate.sol:7129:5: Warning: No visibility specified. Defaulting to "public". In interfaces it defaults to external.
    function setHash(bytes32 node, bytes32 hash);
    ^-------------------------------------------^
,./templates/reputation/contracts/flat_ReputationTemplate.sol:3575:5: Warning: Function state mutability can be restricted to pure
    function getMaxPeriodTransitions() internal view returns (uint64) { return MAX_UINT64; }
    ^--------------------------------------------------------------------------------------^
,@aragon/apps-finance/contracts/Finance.sol:840:5: Warning: Function state mutability can be restricted to pure
    function getMaxPeriodTransitions() internal view returns (uint64) { return MAX_UINT64; }
    ^--------------------------------------------------------------------------------------^

Writing artifacts to ./build/contracts
```

## Trust

```console
$ npx truffle compile

Compiling ./contracts/MultiSigWallet.sol...
Compiling ./contracts/TrustTemplate.sol...
Compiling ./contracts/flat_MultiSigWallet.sol...
Compiling ./contracts/flat_TrustTemplate.sol...
Compiling ./contracts/test/TestImports.sol...
Compiling @aragon/apps-agent/contracts/Agent.sol...
Compiling @aragon/apps-agent/contracts/SignatureValidator.sol...
Compiling @aragon/apps-agent/contracts/standards/ERC1271.sol...
Compiling @aragon/apps-agent/contracts/standards/IERC165.sol...
Compiling @aragon/apps-finance/contracts/Finance.sol...
Compiling @aragon/apps-payroll/contracts/Payroll.sol...
Compiling @aragon/apps-shared-minime/contracts/ITokenController.sol...
Compiling @aragon/apps-shared-minime/contracts/MiniMeToken.sol...
Compiling @aragon/apps-survey/contracts/Survey.sol...
Compiling @aragon/apps-token-manager/contracts/TokenManager.sol...
Compiling @aragon/apps-vault/contracts/Vault.sol...
Compiling @aragon/apps-voting/contracts/Voting.sol...
Compiling @aragon/id/contracts/FIFSResolvingRegistrar.sol...
Compiling @aragon/id/contracts/IFIFSResolvingRegistrar.sol...
Compiling @aragon/id/contracts/ens/IPublicResolver.sol...
Compiling @aragon/os/contracts/acl/ACL.sol...
Compiling @aragon/os/contracts/acl/ACLSyntaxSugar.sol...
Compiling @aragon/os/contracts/acl/IACL.sol...
Compiling @aragon/os/contracts/acl/IACLOracle.sol...
Compiling @aragon/os/contracts/apm/APMNamehash.sol...
Compiling @aragon/os/contracts/apm/APMRegistry.sol...
Compiling @aragon/os/contracts/apm/Repo.sol...
Compiling @aragon/os/contracts/apps/AppProxyBase.sol...
Compiling @aragon/os/contracts/apps/AppProxyPinned.sol...
Compiling @aragon/os/contracts/apps/AppProxyUpgradeable.sol...
Compiling @aragon/os/contracts/apps/AppStorage.sol...
Compiling @aragon/os/contracts/apps/AragonApp.sol...
Compiling @aragon/os/contracts/common/Autopetrified.sol...
Compiling @aragon/os/contracts/common/ConversionHelpers.sol...
Compiling @aragon/os/contracts/common/DelegateProxy.sol...
Compiling @aragon/os/contracts/common/DepositableDelegateProxy.sol...
Compiling @aragon/os/contracts/common/DepositableStorage.sol...
Compiling @aragon/os/contracts/common/EtherTokenConstant.sol...
Compiling @aragon/os/contracts/common/IForwarder.sol...
Compiling @aragon/os/contracts/common/IVaultRecoverable.sol...
Compiling @aragon/os/contracts/common/Initializable.sol...
Compiling @aragon/os/contracts/common/IsContract.sol...
Compiling @aragon/os/contracts/common/Petrifiable.sol...
Compiling @aragon/os/contracts/common/ReentrancyGuard.sol...
Compiling @aragon/os/contracts/common/SafeERC20.sol...
Compiling @aragon/os/contracts/common/TimeHelpers.sol...
Compiling @aragon/os/contracts/common/Uint256Helpers.sol...
Compiling @aragon/os/contracts/common/UnstructuredStorage.sol...
Compiling @aragon/os/contracts/common/VaultRecoverable.sol...
Compiling @aragon/os/contracts/ens/ENSConstants.sol...
Compiling @aragon/os/contracts/ens/ENSSubdomainRegistrar.sol...
Compiling @aragon/os/contracts/evmscript/EVMScriptRegistry.sol...
Compiling @aragon/os/contracts/evmscript/EVMScriptRunner.sol...
Compiling @aragon/os/contracts/evmscript/IEVMScriptExecutor.sol...
Compiling @aragon/os/contracts/evmscript/IEVMScriptRegistry.sol...
Compiling @aragon/os/contracts/evmscript/ScriptHelpers.sol...
Compiling @aragon/os/contracts/evmscript/executors/BaseEVMScriptExecutor.sol...
Compiling @aragon/os/contracts/evmscript/executors/CallsScript.sol...
Compiling @aragon/os/contracts/factory/APMRegistryFactory.sol...
Compiling @aragon/os/contracts/factory/AppProxyFactory.sol...
Compiling @aragon/os/contracts/factory/DAOFactory.sol...
Compiling @aragon/os/contracts/factory/ENSFactory.sol...
Compiling @aragon/os/contracts/factory/EVMScriptRegistryFactory.sol...
Compiling @aragon/os/contracts/kernel/IKernel.sol...
Compiling @aragon/os/contracts/kernel/Kernel.sol...
Compiling @aragon/os/contracts/kernel/KernelConstants.sol...
Compiling @aragon/os/contracts/kernel/KernelProxy.sol...
Compiling @aragon/os/contracts/kernel/KernelStorage.sol...
Compiling @aragon/os/contracts/lib/ens/AbstractENS.sol...
Compiling @aragon/os/contracts/lib/ens/ENS.sol...
Compiling @aragon/os/contracts/lib/ens/PublicResolver.sol...
Compiling @aragon/os/contracts/lib/math/SafeMath.sol...
Compiling @aragon/os/contracts/lib/math/SafeMath64.sol...
Compiling @aragon/os/contracts/lib/misc/ERCProxy.sol...
Compiling @aragon/os/contracts/lib/token/ERC20.sol...
Compiling @aragon/ppf-contracts/contracts/IFeed.sol...
Compiling @aragon/templates-shared/contracts/BaseTemplate.sol...
Compiling @aragon/templates-shared/contracts/Migrations.sol...

Compilation warnings encountered:

./templates/trust/contracts/MultiSigWallet.sol:109:5: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
    function MultiSigWallet(address[] _owners, uint _required)
    ^ (Relevant source part starts here and spans across multiple lines).
,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:37:5: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
    function Controlled()  public { controller = msg.sender;}
    ^-------------------------------------------------------^
,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:123:5: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
    function MiniMeToken(
    ^ (Relevant source part starts here and spans across multiple lines).
,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:195:9: Warning: Use of the "var" keyword is deprecated.
        var previousBalanceFrom = balanceOfAt(_from, block.number);
        ^---------------------^
,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:209:9: Warning: Use of the "var" keyword is deprecated.
        var previousBalanceTo = balanceOfAt(_to, block.number);
        ^-------------------^
,@aragon/os/contracts/lib/ens/ENS.sol:22:48: Warning: "throw" is deprecated in favour of "revert()", "require()" and "assert()".
        if (records[node].owner != msg.sender) throw;
                                               ^---^
,@aragon/os/contracts/lib/ens/ENS.sol:29:5: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
    function ENS() public {
    ^ (Relevant source part starts here and spans across multiple lines).
,@aragon/os/contracts/lib/ens/ENS.sol:73:9: Warning: Use of the "var" keyword is deprecated.
        var subnode = keccak256(node, label);
        ^---------^
,@aragon/os/contracts/lib/ens/PublicResolver.sol:45:44: Warning: "throw" is deprecated in favour of "revert()", "require()" and "assert()".
        if (ens.owner(node) != msg.sender) throw;
                                           ^---^
,@aragon/os/contracts/lib/ens/PublicResolver.sol:53:5: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
    function PublicResolver(AbstractENS ensAddr) public {
    ^ (Relevant source part starts here and spans across multiple lines).
,@aragon/os/contracts/lib/ens/PublicResolver.sol:146:9: Warning: Use of the "var" keyword is deprecated.
        var record = records[node];
        ^--------^
,@aragon/os/contracts/lib/ens/PublicResolver.sol:166:53: Warning: "throw" is deprecated in favour of "revert()", "require()" and "assert()".
        if (((contentType - 1) & contentType) != 0) throw;
                                                    ^---^
,./templates/trust/contracts/flat_MultiSigWallet.sol:112:5: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
    function MultiSigWallet(address[] _owners, uint _required)
    ^ (Relevant source part starts here and spans across multiple lines).
,./templates/trust/contracts/flat_TrustTemplate.sol:3214:5: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
    function Controlled()  public { controller = msg.sender;}
    ^-------------------------------------------------------^
,./templates/trust/contracts/flat_TrustTemplate.sol:3300:5: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
    function MiniMeToken(
    ^ (Relevant source part starts here and spans across multiple lines).
,./templates/trust/contracts/flat_TrustTemplate.sol:3372:9: Warning: Use of the "var" keyword is deprecated.
        var previousBalanceFrom = balanceOfAt(_from, block.number);
        ^---------------------^
,./templates/trust/contracts/flat_TrustTemplate.sol:3386:9: Warning: Use of the "var" keyword is deprecated.
        var previousBalanceTo = balanceOfAt(_to, block.number);
        ^-------------------^
,./templates/trust/contracts/flat_TrustTemplate.sol:6802:48: Warning: "throw" is deprecated in favour of "revert()", "require()" and "assert()".
        if (records[node].owner != msg.sender) throw;
                                               ^---^
,./templates/trust/contracts/flat_TrustTemplate.sol:6809:5: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
    function ENS() public {
    ^ (Relevant source part starts here and spans across multiple lines).
,./templates/trust/contracts/flat_TrustTemplate.sol:6853:9: Warning: Use of the "var" keyword is deprecated.
        var subnode = keccak256(node, label);
        ^---------^
,./templates/trust/contracts/flat_TrustTemplate.sol:6924:44: Warning: "throw" is deprecated in favour of "revert()", "require()" and "assert()".
        if (ens.owner(node) != msg.sender) throw;
                                           ^---^
,./templates/trust/contracts/flat_TrustTemplate.sol:6932:5: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
    function PublicResolver(AbstractENS ensAddr) public {
    ^ (Relevant source part starts here and spans across multiple lines).
,./templates/trust/contracts/flat_TrustTemplate.sol:7025:9: Warning: Use of the "var" keyword is deprecated.
        var record = records[node];
        ^--------^
,./templates/trust/contracts/flat_TrustTemplate.sol:7045:53: Warning: "throw" is deprecated in favour of "revert()", "require()" and "assert()".
        if (((contentType - 1) & contentType) != 0) throw;
                                                    ^---^
,./templates/trust/contracts/flat_TrustTemplate.sol:7567:5: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
    function MultiSigWallet(address[] _owners, uint _required)
    ^ (Relevant source part starts here and spans across multiple lines).
,@aragon/templates-shared/contracts/Migrations.sol:11:3: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
  function Migrations() public {
  ^ (Relevant source part starts here and spans across multiple lines).
,@aragon/os/contracts/lib/ens/ENS.sol:60:37: Warning: This declaration shadows an existing declaration.
    function setOwner(bytes32 node, address owner) only_owner(node) public {
                                    ^-----------^
@aragon/os/contracts/lib/ens/ENS.sol:36:5: The shadowed declaration is here:
    function owner(bytes32 node) public constant returns (address) {
    ^ (Relevant source part starts here and spans across multiple lines).

,@aragon/os/contracts/lib/ens/ENS.sol:72:59: Warning: This declaration shadows an existing declaration.
    function setSubnodeOwner(bytes32 node, bytes32 label, address owner) only_owner(node) public {
                                                          ^-----------^
@aragon/os/contracts/lib/ens/ENS.sol:36:5: The shadowed declaration is here:
    function owner(bytes32 node) public constant returns (address) {
    ^ (Relevant source part starts here and spans across multiple lines).

,@aragon/os/contracts/lib/ens/ENS.sol:83:40: Warning: This declaration shadows an existing declaration.
    function setResolver(bytes32 node, address resolver) only_owner(node) public {
                                       ^--------------^
@aragon/os/contracts/lib/ens/ENS.sol:43:5: The shadowed declaration is here:
    function resolver(bytes32 node) public constant returns (address) {
    ^ (Relevant source part starts here and spans across multiple lines).

,@aragon/os/contracts/lib/ens/ENS.sol:93:35: Warning: This declaration shadows an existing declaration.
    function setTTL(bytes32 node, uint64 ttl) only_owner(node) public {
                                  ^--------^
@aragon/os/contracts/lib/ens/ENS.sol:50:5: The shadowed declaration is here:
    function ttl(bytes32 node) public constant returns (uint64) {
    ^ (Relevant source part starts here and spans across multiple lines).

,@aragon/os/contracts/lib/ens/PublicResolver.sol:87:36: Warning: This declaration shadows an existing declaration.
    function setAddr(bytes32 node, address addr) only_owner(node) public {
                                   ^----------^
@aragon/os/contracts/lib/ens/PublicResolver.sol:77:5: The shadowed declaration is here:
    function addr(bytes32 node) public constant returns (address ret) {
    ^ (Relevant source part starts here and spans across multiple lines).

,@aragon/os/contracts/lib/ens/PublicResolver.sol:132:36: Warning: This declaration shadows an existing declaration.
    function setName(bytes32 node, string name) only_owner(node) public {
                                   ^---------^
@aragon/os/contracts/lib/ens/PublicResolver.sol:122:5: The shadowed declaration is here:
    function name(bytes32 node) public constant returns (string ret) {
    ^ (Relevant source part starts here and spans across multiple lines).

,@aragon/id/contracts/ens/IPublicResolver.sol:7:36: Warning: This declaration shadows an existing declaration.
    function setAddr(bytes32 node, address addr);
                                   ^----------^
@aragon/id/contracts/ens/IPublicResolver.sol:6:5: The shadowed declaration is here:
    function addr(bytes32 node) constant returns (address ret);
    ^---------------------------------------------------------^

,@aragon/id/contracts/ens/IPublicResolver.sol:9:36: Warning: This declaration shadows an existing declaration.
    function setHash(bytes32 node, bytes32 hash);
                                   ^----------^
@aragon/id/contracts/ens/IPublicResolver.sol:8:5: The shadowed declaration is here:
    function hash(bytes32 node) constant returns (bytes32 ret);
    ^---------------------------------------------------------^

,./templates/trust/contracts/flat_TrustTemplate.sol:6840:37: Warning: This declaration shadows an existing declaration.
    function setOwner(bytes32 node, address owner) only_owner(node) public {
                                    ^-----------^
./templates/trust/contracts/flat_TrustTemplate.sol:6816:5: The shadowed declaration is here:
    function owner(bytes32 node) public constant returns (address) {
    ^ (Relevant source part starts here and spans across multiple lines).

,./templates/trust/contracts/flat_TrustTemplate.sol:6852:59: Warning: This declaration shadows an existing declaration.
    function setSubnodeOwner(bytes32 node, bytes32 label, address owner) only_owner(node) public {
                                                          ^-----------^
./templates/trust/contracts/flat_TrustTemplate.sol:6816:5: The shadowed declaration is here:
    function owner(bytes32 node) public constant returns (address) {
    ^ (Relevant source part starts here and spans across multiple lines).

,./templates/trust/contracts/flat_TrustTemplate.sol:6863:40: Warning: This declaration shadows an existing declaration.
    function setResolver(bytes32 node, address resolver) only_owner(node) public {
                                       ^--------------^
./templates/trust/contracts/flat_TrustTemplate.sol:6823:5: The shadowed declaration is here:
    function resolver(bytes32 node) public constant returns (address) {
    ^ (Relevant source part starts here and spans across multiple lines).

,./templates/trust/contracts/flat_TrustTemplate.sol:6873:35: Warning: This declaration shadows an existing declaration.
    function setTTL(bytes32 node, uint64 ttl) only_owner(node) public {
                                  ^--------^
./templates/trust/contracts/flat_TrustTemplate.sol:6830:5: The shadowed declaration is here:
    function ttl(bytes32 node) public constant returns (uint64) {
    ^ (Relevant source part starts here and spans across multiple lines).

,./templates/trust/contracts/flat_TrustTemplate.sol:6966:36: Warning: This declaration shadows an existing declaration.
    function setAddr(bytes32 node, address addr) only_owner(node) public {
                                   ^----------^
./templates/trust/contracts/flat_TrustTemplate.sol:6956:5: The shadowed declaration is here:
    function addr(bytes32 node) public constant returns (address ret) {
    ^ (Relevant source part starts here and spans across multiple lines).

,./templates/trust/contracts/flat_TrustTemplate.sol:7011:36: Warning: This declaration shadows an existing declaration.
    function setName(bytes32 node, string name) only_owner(node) public {
                                   ^---------^
./templates/trust/contracts/flat_TrustTemplate.sol:7001:5: The shadowed declaration is here:
    function name(bytes32 node) public constant returns (string ret) {
    ^ (Relevant source part starts here and spans across multiple lines).

,./templates/trust/contracts/flat_TrustTemplate.sol:7103:36: Warning: This declaration shadows an existing declaration.
    function setAddr(bytes32 node, address addr);
                                   ^----------^
./templates/trust/contracts/flat_TrustTemplate.sol:7102:5: The shadowed declaration is here:
    function addr(bytes32 node) constant returns (address ret);
    ^---------------------------------------------------------^

,./templates/trust/contracts/flat_TrustTemplate.sol:7105:36: Warning: This declaration shadows an existing declaration.
    function setHash(bytes32 node, bytes32 hash);
                                   ^----------^
./templates/trust/contracts/flat_TrustTemplate.sol:7104:5: The shadowed declaration is here:
    function hash(bytes32 node) constant returns (bytes32 ret);
    ^---------------------------------------------------------^

,@aragon/apps-vault/contracts/Vault.sol:76:5: Warning: Variable is shadowed in inline assembly by an instruction of the same name
    function balance(address _token) public view returns (uint256) {
    ^ (Relevant source part starts here and spans across multiple lines).
,@aragon/apps-vault/contracts/Vault.sol:76:5: Warning: Variable is shadowed in inline assembly by an instruction of the same name
    function balance(address _token) public view returns (uint256) {
    ^ (Relevant source part starts here and spans across multiple lines).
,./templates/trust/contracts/flat_TrustTemplate.sol:2865:5: Warning: Variable is shadowed in inline assembly by an instruction of the same name
    function balance(address _token) public view returns (uint256) {
    ^ (Relevant source part starts here and spans across multiple lines).
,./templates/trust/contracts/flat_TrustTemplate.sol:2865:5: Warning: Variable is shadowed in inline assembly by an instruction of the same name
    function balance(address _token) public view returns (uint256) {
    ^ (Relevant source part starts here and spans across multiple lines).
,./templates/trust/contracts/MultiSigWallet.sol:100:13: Warning: Invoking events without "emit" prefix is deprecated.
            Deposit(msg.sender, msg.value);
            ^----------------------------^
,./templates/trust/contracts/MultiSigWallet.sol:132:9: Warning: Invoking events without "emit" prefix is deprecated.
        OwnerAddition(owner);
        ^------------------^
,./templates/trust/contracts/MultiSigWallet.sol:151:9: Warning: Invoking events without "emit" prefix is deprecated.
        OwnerRemoval(owner);
        ^-----------------^
,./templates/trust/contracts/MultiSigWallet.sol:170:9: Warning: Invoking events without "emit" prefix is deprecated.
        OwnerRemoval(owner);
        ^-----------------^
,./templates/trust/contracts/MultiSigWallet.sol:171:9: Warning: Invoking events without "emit" prefix is deprecated.
        OwnerAddition(newOwner);
        ^---------------------^
,./templates/trust/contracts/MultiSigWallet.sol:182:9: Warning: Invoking events without "emit" prefix is deprecated.
        RequirementChange(_required);
        ^--------------------------^
,./templates/trust/contracts/MultiSigWallet.sol:207:9: Warning: Invoking events without "emit" prefix is deprecated.
        Confirmation(msg.sender, transactionId);
        ^-------------------------------------^
,./templates/trust/contracts/MultiSigWallet.sol:220:9: Warning: Invoking events without "emit" prefix is deprecated.
        Revocation(msg.sender, transactionId);
        ^-----------------------------------^
,./templates/trust/contracts/MultiSigWallet.sol:235:17: Warning: Invoking events without "emit" prefix is deprecated.
                Execution(transactionId);
                ^----------------------^
,./templates/trust/contracts/MultiSigWallet.sol:237:17: Warning: Invoking events without "emit" prefix is deprecated.
                ExecutionFailure(transactionId);
                ^-----------------------------^
,./templates/trust/contracts/MultiSigWallet.sol:303:9: Warning: Invoking events without "emit" prefix is deprecated.
        Submission(transactionId);
        ^-----------------------^
,@aragon/os/contracts/acl/IACL.sol:13:5: Warning: Functions in interfaces should be declared external.
    function hasPermission(address who, address where, bytes32 what, bytes how) public view returns (bool);
    ^-----------------------------------------------------------------------------------------------------^
,@aragon/os/contracts/evmscript/IEVMScriptRegistry.sol:24:5: Warning: Functions in interfaces should be declared external.
    function getScriptExecutor(bytes script) public view returns (IEVMScriptExecutor);
    ^--------------------------------------------------------------------------------^
,@aragon/os/contracts/common/IForwarder.sol:13:5: Warning: Functions in interfaces should be declared external.
    function canForward(address sender, bytes evmCallScript) public view returns (bool);
    ^----------------------------------------------------------------------------------^
,@aragon/os/contracts/common/IForwarder.sol:17:5: Warning: Functions in interfaces should be declared external.
    function forward(bytes evmCallScript) public;
    ^-------------------------------------------^
,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:213:9: Warning: Invoking events without "emit" prefix is deprecated.
        Transfer(_from, _to, _amount);
        ^---------------------------^
,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:245:9: Warning: Invoking events without "emit" prefix is deprecated.
        Approval(msg.sender, _spender, _amount);
        ^-------------------------------------^
,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:373:9: Warning: Invoking events without "emit" prefix is deprecated.
        NewCloneToken(address(cloneToken), snapshot);
        ^------------------------------------------^
,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:392:9: Warning: Invoking events without "emit" prefix is deprecated.
        Transfer(0, _owner, _amount);
        ^--------------------------^
,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:408:9: Warning: Invoking events without "emit" prefix is deprecated.
        Transfer(_owner, 0, _amount);
        ^--------------------------^
,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:509:33: Warning: Using contract member "balance" inherited from the address type is deprecated. Convert the contract to "address" type to access the member, for example use "address(contract).balance" instead.
            controller.transfer(this.balance);
                                ^----------^
,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:516:9: Warning: Invoking events without "emit" prefix is deprecated.
        ClaimedTokens(_token, controller, balance);
        ^----------------------------------------^
,@aragon/os/contracts/lib/ens/AbstractENS.sol:7:5: Warning: Functions in interfaces should be declared external.
    function owner(bytes32 _node) public constant returns (address);
    ^--------------------------------------------------------------^
,@aragon/os/contracts/lib/ens/AbstractENS.sol:8:5: Warning: Functions in interfaces should be declared external.
    function resolver(bytes32 _node) public constant returns (address);
    ^-----------------------------------------------------------------^
,@aragon/os/contracts/lib/ens/AbstractENS.sol:9:5: Warning: Functions in interfaces should be declared external.
    function ttl(bytes32 _node) public constant returns (uint64);
    ^-----------------------------------------------------------^
,@aragon/os/contracts/lib/ens/AbstractENS.sol:10:5: Warning: Functions in interfaces should be declared external.
    function setOwner(bytes32 _node, address _owner) public;
    ^------------------------------------------------------^
,@aragon/os/contracts/lib/ens/AbstractENS.sol:11:5: Warning: Functions in interfaces should be declared external.
    function setSubnodeOwner(bytes32 _node, bytes32 label, address _owner) public;
    ^----------------------------------------------------------------------------^
,@aragon/os/contracts/lib/ens/AbstractENS.sol:12:5: Warning: Functions in interfaces should be declared external.
    function setResolver(bytes32 _node, address _resolver) public;
    ^------------------------------------------------------------^
,@aragon/os/contracts/lib/ens/AbstractENS.sol:13:5: Warning: Functions in interfaces should be declared external.
    function setTTL(bytes32 _node, uint64 _ttl) public;
    ^-------------------------------------------------^
,@aragon/os/contracts/lib/ens/ENS.sol:30:17: Warning: Decimal literal assigned to bytesXX variable will be left-aligned. Use an explicit conversion to silence this warning.
        records[0].owner = msg.sender;
                ^
,@aragon/os/contracts/lib/ens/ENS.sol:61:9: Warning: Invoking events without "emit" prefix is deprecated.
        Transfer(node, owner);
        ^-------------------^
,@aragon/os/contracts/lib/ens/ENS.sol:73:23: Warning: This function only accepts a single "bytes" argument. Please use "abi.encodePacked(...)" or a similar function to encode the data.
        var subnode = keccak256(node, label);
                      ^--------------------^
,@aragon/os/contracts/lib/ens/ENS.sol:74:9: Warning: Invoking events without "emit" prefix is deprecated.
        NewOwner(node, label, owner);
        ^--------------------------^
,@aragon/os/contracts/lib/ens/ENS.sol:84:9: Warning: Invoking events without "emit" prefix is deprecated.
        NewResolver(node, resolver);
        ^-------------------------^
,@aragon/os/contracts/lib/ens/ENS.sol:94:9: Warning: Invoking events without "emit" prefix is deprecated.
        NewTTL(node, ttl);
        ^---------------^
,@aragon/os/contracts/lib/ens/PublicResolver.sol:89:9: Warning: Invoking events without "emit" prefix is deprecated.
        AddrChanged(node, addr);
        ^---------------------^
,@aragon/os/contracts/lib/ens/PublicResolver.sol:113:9: Warning: Invoking events without "emit" prefix is deprecated.
        ContentChanged(node, hash);
        ^------------------------^
,@aragon/os/contracts/lib/ens/PublicResolver.sol:134:9: Warning: Invoking events without "emit" prefix is deprecated.
        NameChanged(node, name);
        ^---------------------^
,@aragon/os/contracts/lib/ens/PublicResolver.sol:169:9: Warning: Invoking events without "emit" prefix is deprecated.
        ABIChanged(node, contentType);
        ^---------------------------^
,@aragon/os/contracts/lib/ens/PublicResolver.sol:190:9: Warning: Invoking events without "emit" prefix is deprecated.
        PubkeyChanged(node, x, y);
        ^-----------------------^
,@aragon/os/contracts/lib/ens/PublicResolver.sol:212:9: Warning: Invoking events without "emit" prefix is deprecated.
        TextChanged(node, key, key);
        ^-------------------------^
,@aragon/id/contracts/ens/IPublicResolver.sol:5:5: Warning: Functions in interfaces should be declared external.
    function supportsInterface(bytes4 interfaceID) constant returns (bool);
    ^---------------------------------------------------------------------^
,@aragon/id/contracts/ens/IPublicResolver.sol:6:5: Warning: Functions in interfaces should be declared external.
    function addr(bytes32 node) constant returns (address ret);
    ^---------------------------------------------------------^
,@aragon/id/contracts/ens/IPublicResolver.sol:7:5: Warning: Functions in interfaces should be declared external.
    function setAddr(bytes32 node, address addr);
    ^-------------------------------------------^
,@aragon/id/contracts/ens/IPublicResolver.sol:8:5: Warning: Functions in interfaces should be declared external.
    function hash(bytes32 node) constant returns (bytes32 ret);
    ^---------------------------------------------------------^
,@aragon/id/contracts/ens/IPublicResolver.sol:9:5: Warning: Functions in interfaces should be declared external.
    function setHash(bytes32 node, bytes32 hash);
    ^-------------------------------------------^
,@aragon/id/contracts/IFIFSResolvingRegistrar.sol:8:5: Warning: Functions in interfaces should be declared external.
    function registerWithResolver(bytes32 _subnode, address _owner, IPublicResolver _resolver) public;
    ^------------------------------------------------------------------------------------------------^
,./templates/trust/contracts/flat_MultiSigWallet.sol:103:13: Warning: Invoking events without "emit" prefix is deprecated.
            Deposit(msg.sender, msg.value);
            ^----------------------------^
,./templates/trust/contracts/flat_MultiSigWallet.sol:135:9: Warning: Invoking events without "emit" prefix is deprecated.
        OwnerAddition(owner);
        ^------------------^
,./templates/trust/contracts/flat_MultiSigWallet.sol:154:9: Warning: Invoking events without "emit" prefix is deprecated.
        OwnerRemoval(owner);
        ^-----------------^
,./templates/trust/contracts/flat_MultiSigWallet.sol:173:9: Warning: Invoking events without "emit" prefix is deprecated.
        OwnerRemoval(owner);
        ^-----------------^
,./templates/trust/contracts/flat_MultiSigWallet.sol:174:9: Warning: Invoking events without "emit" prefix is deprecated.
        OwnerAddition(newOwner);
        ^---------------------^
,./templates/trust/contracts/flat_MultiSigWallet.sol:185:9: Warning: Invoking events without "emit" prefix is deprecated.
        RequirementChange(_required);
        ^--------------------------^
,./templates/trust/contracts/flat_MultiSigWallet.sol:210:9: Warning: Invoking events without "emit" prefix is deprecated.
        Confirmation(msg.sender, transactionId);
        ^-------------------------------------^
,./templates/trust/contracts/flat_MultiSigWallet.sol:223:9: Warning: Invoking events without "emit" prefix is deprecated.
        Revocation(msg.sender, transactionId);
        ^-----------------------------------^
,./templates/trust/contracts/flat_MultiSigWallet.sol:238:17: Warning: Invoking events without "emit" prefix is deprecated.
                Execution(transactionId);
                ^----------------------^
,./templates/trust/contracts/flat_MultiSigWallet.sol:240:17: Warning: Invoking events without "emit" prefix is deprecated.
                ExecutionFailure(transactionId);
                ^-----------------------------^
,./templates/trust/contracts/flat_MultiSigWallet.sol:306:9: Warning: Invoking events without "emit" prefix is deprecated.
        Submission(transactionId);
        ^-----------------------^
,./templates/trust/contracts/flat_TrustTemplate.sol:59:5: Warning: Functions in interfaces should be declared external.
    function hasPermission(address who, address where, bytes32 what, bytes how) public view returns (bool);
    ^-----------------------------------------------------------------------------------------------------^
,./templates/trust/contracts/flat_TrustTemplate.sol:826:5: Warning: Functions in interfaces should be declared external.
    function getScriptExecutor(bytes script) public view returns (IEVMScriptExecutor);
    ^--------------------------------------------------------------------------------^
,./templates/trust/contracts/flat_TrustTemplate.sol:2913:5: Warning: Functions in interfaces should be declared external.
    function canForward(address sender, bytes evmCallScript) public view returns (bool);
    ^----------------------------------------------------------------------------------^
,./templates/trust/contracts/flat_TrustTemplate.sol:2917:5: Warning: Functions in interfaces should be declared external.
    function forward(bytes evmCallScript) public;
    ^-------------------------------------------^
,./templates/trust/contracts/flat_TrustTemplate.sol:3390:9: Warning: Invoking events without "emit" prefix is deprecated.
        Transfer(_from, _to, _amount);
        ^---------------------------^
,./templates/trust/contracts/flat_TrustTemplate.sol:3422:9: Warning: Invoking events without "emit" prefix is deprecated.
        Approval(msg.sender, _spender, _amount);
        ^-------------------------------------^
,./templates/trust/contracts/flat_TrustTemplate.sol:3550:9: Warning: Invoking events without "emit" prefix is deprecated.
        NewCloneToken(address(cloneToken), snapshot);
        ^------------------------------------------^
,./templates/trust/contracts/flat_TrustTemplate.sol:3569:9: Warning: Invoking events without "emit" prefix is deprecated.
        Transfer(0, _owner, _amount);
        ^--------------------------^
,./templates/trust/contracts/flat_TrustTemplate.sol:3585:9: Warning: Invoking events without "emit" prefix is deprecated.
        Transfer(_owner, 0, _amount);
        ^--------------------------^
,./templates/trust/contracts/flat_TrustTemplate.sol:3686:33: Warning: Using contract member "balance" inherited from the address type is deprecated. Convert the contract to "address" type to access the member, for example use "address(contract).balance" instead.
            controller.transfer(this.balance);
                                ^----------^
,./templates/trust/contracts/flat_TrustTemplate.sol:3693:9: Warning: Invoking events without "emit" prefix is deprecated.
        ClaimedTokens(_token, controller, balance);
        ^----------------------------------------^
,./templates/trust/contracts/flat_TrustTemplate.sol:6760:5: Warning: Functions in interfaces should be declared external.
    function owner(bytes32 _node) public constant returns (address);
    ^--------------------------------------------------------------^
,./templates/trust/contracts/flat_TrustTemplate.sol:6761:5: Warning: Functions in interfaces should be declared external.
    function resolver(bytes32 _node) public constant returns (address);
    ^-----------------------------------------------------------------^
,./templates/trust/contracts/flat_TrustTemplate.sol:6762:5: Warning: Functions in interfaces should be declared external.
    function ttl(bytes32 _node) public constant returns (uint64);
    ^-----------------------------------------------------------^
,./templates/trust/contracts/flat_TrustTemplate.sol:6763:5: Warning: Functions in interfaces should be declared external.
    function setOwner(bytes32 _node, address _owner) public;
    ^------------------------------------------------------^
,./templates/trust/contracts/flat_TrustTemplate.sol:6764:5: Warning: Functions in interfaces should be declared external.
    function setSubnodeOwner(bytes32 _node, bytes32 label, address _owner) public;
    ^----------------------------------------------------------------------------^
,./templates/trust/contracts/flat_TrustTemplate.sol:6765:5: Warning: Functions in interfaces should be declared external.
    function setResolver(bytes32 _node, address _resolver) public;
    ^------------------------------------------------------------^
,./templates/trust/contracts/flat_TrustTemplate.sol:6766:5: Warning: Functions in interfaces should be declared external.
    function setTTL(bytes32 _node, uint64 _ttl) public;
    ^-------------------------------------------------^
,./templates/trust/contracts/flat_TrustTemplate.sol:6810:17: Warning: Decimal literal assigned to bytesXX variable will be left-aligned. Use an explicit conversion to silence this warning.
        records[0].owner = msg.sender;
                ^
,./templates/trust/contracts/flat_TrustTemplate.sol:6841:9: Warning: Invoking events without "emit" prefix is deprecated.
        Transfer(node, owner);
        ^-------------------^
,./templates/trust/contracts/flat_TrustTemplate.sol:6853:23: Warning: This function only accepts a single "bytes" argument. Please use "abi.encodePacked(...)" or a similar function to encode the data.
        var subnode = keccak256(node, label);
                      ^--------------------^
,./templates/trust/contracts/flat_TrustTemplate.sol:6854:9: Warning: Invoking events without "emit" prefix is deprecated.
        NewOwner(node, label, owner);
        ^--------------------------^
,./templates/trust/contracts/flat_TrustTemplate.sol:6864:9: Warning: Invoking events without "emit" prefix is deprecated.
        NewResolver(node, resolver);
        ^-------------------------^
,./templates/trust/contracts/flat_TrustTemplate.sol:6874:9: Warning: Invoking events without "emit" prefix is deprecated.
        NewTTL(node, ttl);
        ^---------------^
,./templates/trust/contracts/flat_TrustTemplate.sol:6968:9: Warning: Invoking events without "emit" prefix is deprecated.
        AddrChanged(node, addr);
        ^---------------------^
,./templates/trust/contracts/flat_TrustTemplate.sol:6992:9: Warning: Invoking events without "emit" prefix is deprecated.
        ContentChanged(node, hash);
        ^------------------------^
,./templates/trust/contracts/flat_TrustTemplate.sol:7013:9: Warning: Invoking events without "emit" prefix is deprecated.
        NameChanged(node, name);
        ^---------------------^
,./templates/trust/contracts/flat_TrustTemplate.sol:7048:9: Warning: Invoking events without "emit" prefix is deprecated.
        ABIChanged(node, contentType);
        ^---------------------------^
,./templates/trust/contracts/flat_TrustTemplate.sol:7069:9: Warning: Invoking events without "emit" prefix is deprecated.
        PubkeyChanged(node, x, y);
        ^-----------------------^
,./templates/trust/contracts/flat_TrustTemplate.sol:7091:9: Warning: Invoking events without "emit" prefix is deprecated.
        TextChanged(node, key, key);
        ^-------------------------^
,./templates/trust/contracts/flat_TrustTemplate.sol:7101:5: Warning: Functions in interfaces should be declared external.
    function supportsInterface(bytes4 interfaceID) constant returns (bool);
    ^---------------------------------------------------------------------^
,./templates/trust/contracts/flat_TrustTemplate.sol:7102:5: Warning: Functions in interfaces should be declared external.
    function addr(bytes32 node) constant returns (address ret);
    ^---------------------------------------------------------^
,./templates/trust/contracts/flat_TrustTemplate.sol:7103:5: Warning: Functions in interfaces should be declared external.
    function setAddr(bytes32 node, address addr);
    ^-------------------------------------------^
,./templates/trust/contracts/flat_TrustTemplate.sol:7104:5: Warning: Functions in interfaces should be declared external.
    function hash(bytes32 node) constant returns (bytes32 ret);
    ^---------------------------------------------------------^
,./templates/trust/contracts/flat_TrustTemplate.sol:7105:5: Warning: Functions in interfaces should be declared external.
    function setHash(bytes32 node, bytes32 hash);
    ^-------------------------------------------^
,./templates/trust/contracts/flat_TrustTemplate.sol:7116:5: Warning: Functions in interfaces should be declared external.
    function registerWithResolver(bytes32 _subnode, address _owner, IPublicResolver _resolver) public;
    ^------------------------------------------------------------------------------------------------^
,./templates/trust/contracts/flat_TrustTemplate.sol:7558:13: Warning: Invoking events without "emit" prefix is deprecated.
            Deposit(msg.sender, msg.value);
            ^----------------------------^
,./templates/trust/contracts/flat_TrustTemplate.sol:7590:9: Warning: Invoking events without "emit" prefix is deprecated.
        OwnerAddition(owner);
        ^------------------^
,./templates/trust/contracts/flat_TrustTemplate.sol:7609:9: Warning: Invoking events without "emit" prefix is deprecated.
        OwnerRemoval(owner);
        ^-----------------^
,./templates/trust/contracts/flat_TrustTemplate.sol:7628:9: Warning: Invoking events without "emit" prefix is deprecated.
        OwnerRemoval(owner);
        ^-----------------^
,./templates/trust/contracts/flat_TrustTemplate.sol:7629:9: Warning: Invoking events without "emit" prefix is deprecated.
        OwnerAddition(newOwner);
        ^---------------------^
,./templates/trust/contracts/flat_TrustTemplate.sol:7640:9: Warning: Invoking events without "emit" prefix is deprecated.
        RequirementChange(_required);
        ^--------------------------^
,./templates/trust/contracts/flat_TrustTemplate.sol:7665:9: Warning: Invoking events without "emit" prefix is deprecated.
        Confirmation(msg.sender, transactionId);
        ^-------------------------------------^
,./templates/trust/contracts/flat_TrustTemplate.sol:7678:9: Warning: Invoking events without "emit" prefix is deprecated.
        Revocation(msg.sender, transactionId);
        ^-----------------------------------^
,./templates/trust/contracts/flat_TrustTemplate.sol:7693:17: Warning: Invoking events without "emit" prefix is deprecated.
                Execution(transactionId);
                ^----------------------^
,./templates/trust/contracts/flat_TrustTemplate.sol:7695:17: Warning: Invoking events without "emit" prefix is deprecated.
                ExecutionFailure(transactionId);
                ^-----------------------------^
,./templates/trust/contracts/flat_TrustTemplate.sol:7761:9: Warning: Invoking events without "emit" prefix is deprecated.
        Submission(transactionId);
        ^-----------------------^
,@aragon/id/contracts/FIFSResolvingRegistrar.sol:55:24: Warning: This function only accepts a single "bytes" argument. Please use "abi.encodePacked(...)" or a similar function to encode the data.
        bytes32 node = keccak256(rootNode, _subnode);
                       ^---------------------------^
,./templates/trust/contracts/MultiSigWallet.sol:96:5: Warning: No visibility specified. Defaulting to "public". 
    function()
    ^ (Relevant source part starts here and spans across multiple lines).
,@aragon/os/contracts/common/VaultRecoverable.sol:49:34: Warning: Unused function parameter. Remove or comment out the variable name to silence this warning.
    function allowRecoverability(address token) public view returns (bool) {
                                 ^-----------^
,@aragon/id/contracts/ens/IPublicResolver.sol:5:5: Warning: No visibility specified. Defaulting to "public". In interfaces it defaults to external.
    function supportsInterface(bytes4 interfaceID) constant returns (bool);
    ^---------------------------------------------------------------------^
,@aragon/id/contracts/ens/IPublicResolver.sol:6:5: Warning: No visibility specified. Defaulting to "public". In interfaces it defaults to external.
    function addr(bytes32 node) constant returns (address ret);
    ^---------------------------------------------------------^
,@aragon/id/contracts/ens/IPublicResolver.sol:7:5: Warning: No visibility specified. Defaulting to "public". In interfaces it defaults to external.
    function setAddr(bytes32 node, address addr);
    ^-------------------------------------------^
,@aragon/id/contracts/ens/IPublicResolver.sol:8:5: Warning: No visibility specified. Defaulting to "public". In interfaces it defaults to external.
    function hash(bytes32 node) constant returns (bytes32 ret);
    ^---------------------------------------------------------^
,@aragon/id/contracts/ens/IPublicResolver.sol:9:5: Warning: No visibility specified. Defaulting to "public". In interfaces it defaults to external.
    function setHash(bytes32 node, bytes32 hash);
    ^-------------------------------------------^
,./templates/trust/contracts/flat_MultiSigWallet.sol:99:5: Warning: No visibility specified. Defaulting to "public". 
    function()
    ^ (Relevant source part starts here and spans across multiple lines).
,./templates/trust/contracts/flat_TrustTemplate.sol:780:34: Warning: Unused function parameter. Remove or comment out the variable name to silence this warning.
    function allowRecoverability(address token) public view returns (bool) {
                                 ^-----------^
,./templates/trust/contracts/flat_TrustTemplate.sol:7101:5: Warning: No visibility specified. Defaulting to "public". In interfaces it defaults to external.
    function supportsInterface(bytes4 interfaceID) constant returns (bool);
    ^---------------------------------------------------------------------^
,./templates/trust/contracts/flat_TrustTemplate.sol:7102:5: Warning: No visibility specified. Defaulting to "public". In interfaces it defaults to external.
    function addr(bytes32 node) constant returns (address ret);
    ^---------------------------------------------------------^
,./templates/trust/contracts/flat_TrustTemplate.sol:7103:5: Warning: No visibility specified. Defaulting to "public". In interfaces it defaults to external.
    function setAddr(bytes32 node, address addr);
    ^-------------------------------------------^
,./templates/trust/contracts/flat_TrustTemplate.sol:7104:5: Warning: No visibility specified. Defaulting to "public". In interfaces it defaults to external.
    function hash(bytes32 node) constant returns (bytes32 ret);
    ^---------------------------------------------------------^
,./templates/trust/contracts/flat_TrustTemplate.sol:7105:5: Warning: No visibility specified. Defaulting to "public". In interfaces it defaults to external.
    function setHash(bytes32 node, bytes32 hash);
    ^-------------------------------------------^
,./templates/trust/contracts/flat_TrustTemplate.sol:7554:5: Warning: No visibility specified. Defaulting to "public". 
    function()
    ^ (Relevant source part starts here and spans across multiple lines).
,./templates/trust/contracts/flat_TrustTemplate.sol:4975:5: Warning: Function state mutability can be restricted to pure
    function getMaxPeriodTransitions() internal view returns (uint64) { return MAX_UINT64; }
    ^--------------------------------------------------------------------------------------^
,@aragon/apps-finance/contracts/Finance.sol:840:5: Warning: Function state mutability can be restricted to pure
    function getMaxPeriodTransitions() internal view returns (uint64) { return MAX_UINT64; }
    ^--------------------------------------------------------------------------------------^

Writing artifacts to ./build/contracts
```