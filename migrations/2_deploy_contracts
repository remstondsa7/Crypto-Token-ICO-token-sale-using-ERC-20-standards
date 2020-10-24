var CryptoToken = artifacts.require("CryptoToken.sol");
var CryptoTokenSale=artifacts.require("CryptoTokenSale.sol");
module.exports = function (deployer) {
  deployer.deploy(CryptoToken, 1000000).then(function() {
    // Token price is 0.001 Ether
    var tokenPrice = 1000000000000000;
    return deployer.deploy(CryptoTokenSale, CryptoToken.address, tokenPrice);
  });
};
