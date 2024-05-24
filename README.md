let numberofRagnaToken = [];
> This code is to declares an empty array named numberofRagnaToken. This array will store objects representing Ragna tokens.

function mintRagnaToken(tokenType, tokenValue, tokenQuantity) {
> This is definition of a function named mintRagnaToken. This function takes three parameters: tokenType, tokenValue, and tokenQuantity, which represent the type, value, and quantity of the Ragna token to be minted.

let newNFT = { tokenType: tokenType, tokenValue: tokenValue, tokenQuantity: tokenQuantity };
> Inside the mintRagnaToken function, this line creates a new object named newNFT. This object has three properties: tokenType, tokenValue, and tokenQuantity, which are assigned values based on the arguments passed to the function.

numberofRagnaToken.push(newNFT);
> This code is for adds the newly created newNFT object to the numberofRagnaToken array using the push method. This effectively adds a new entry to the array, representing the minted Ragna token.

function listRagnaTokens() {
> This code defines a function named listRagnaTokens, which will be used to display the details of all minted Ragna tokens.

numberofRagnaToken.forEach((nft, index) => {
> This code is to starts a loop through each element of the numberofRagnaToken array using the forEach method. For each element, it executes the provided function, passing the current element as nft and its index as index.

console.log(RagnaToken ${index + 1}:);
> This line logs the index of the current Ragna token being displayed. The index starts from 0, so index + 1 is used to display a more human-friendly index starting from 1.

console.log(Type of Token: ${nft.tokenType});
> This code is to logs the type of the current Ragna token being displayed, accessed from the tokenType property of the current nft object.

console.log(Value of Token: ${nft.tokenValue});
> This code is to logs the value of the current Ragna token being displayed, accessed from the tokenValue property of the current nft object.

console.log(Quantity of Token: ${nft.tokenQuantity});
> This code is to logs the quantity of the current Ragna token being displayed, accessed from the tokenQuantity property of the current nft object.

console.log("------------------------------");
> This code is to logs a separator to visually separate the details of different Ragna tokens.

function getTotalRagnaToken() {
> This code is for defines a function named getTotalRagnaToken, which will be used to display the total number of minted Ragna tokens.

console.log(Total number of NFTs minted: ${numberofRagnaToken.length});
> This code is to logs the total number of minted Ragna tokens by accessing the length property of the numberofRagnaToken array.

Function calls mintRagnaToken, listRagnaTokens, and getTotalRagnaToken
> These code is to call the defined functions to MINT Ragna tokens, list them, and display the total count.
