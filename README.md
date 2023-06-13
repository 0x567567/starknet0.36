# starknet0.36
// var decimal = parseInt(response.getContentText(), 16);
  let result = JSON.parse(response.getContentText()).result;
  let decimal = parseInt(result, 16);
  if (isNaN(decimal)) {
    return 0;
  }
  return decimal;
}

// 获取 Token 余额，ERC20 或者 ERC721
function getTokenBalance(walletAddress, contractAddress, network) {
  let rpcLink = RPC_MAP[network];
  if (!rpcLink) {
    return "Error: Invalid Network Name";
 const result = JSON.parse(UrlFetchApp.fetch(api_url));
    const nonce = result["result"]["committed"]["nonce"];
