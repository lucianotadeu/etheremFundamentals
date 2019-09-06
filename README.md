# etheremFundamentals
Geth  - Scripts Prática  Crie uma função "depositar" que receba um valor de ether e um endereço e realize a transferência para o endereço.
> function depositar (valor, origem, destino) {
eth.sendTransaction({from:origem,to:destino, value:web3.toWei(valor)});
console.log(web3.fromWei(eth.getBalance(destino).toString(),"ether"));
};	

> depositar(1,eth.accounts[0], eth.accounts[1])
6
undefined
> depositar(1,eth.accounts[0], eth.accounts[1])
8
undefined
> depositar(1,eth.accounts[0], eth.accounts[1])
9
undefined
> depositar(1,eth.accounts[1], eth.accounts[0])
