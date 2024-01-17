# javascrip

const NFTs = []
function mintNFT(_model, _version, _year, _color) {
	
	const NFT = {
		"model" : _model,
		"version" : _version,
		"year" : _year,
		"color" : _color
	}
	NFTs.push(NFT);
	console.log("Minted: " + _model);
}

// create a "loop" that will go through an "array" of NFT's
// and print their metadata with console.log()
function listNFTs() {
	for(let i = 0;i<NFTs.length;i++) {
    
		console.log("\nmodel: "+NFTs[i].model);
		console.log("version: "+NFTs[i].version);
		console.log("year: "+NFTs[i].year);
		console.log("color: "+NFTs[i].color);
    
	}

}

// print the total number of NFTs we have minted to the console
function getTotalSupply() {
	console.log("Total Supply: "+NFTs.length);
}

// call your functions below this line
mintNFT("NMax", "V2", "2023", "Black");
mintNFT("XMax", "V1", "2022", "Brown");
mintNFT("TMax", "V1", "2023", "Blue");
mintNFT("SMax", "V1", "2019", "Red");
listNFTs();
console.log("\n");
getTotalSupply();
