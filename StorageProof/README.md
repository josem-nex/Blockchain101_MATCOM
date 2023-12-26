# StorageProofVerifier
En el contrato storageProofVerifier de Sepolia, dirección del proxy: `0x3213CB2Ce3342f670a2c1e25F821b99F0655c5a0` e implementacion(storageProofVerifier.sol): `0xa4cFF16CED9268a0f4a630029dAce859bf6623ff` se verificó la propiedad de cada token POAP en la red GNOSIS. En cada clase del curso Blockchain101 cada estudiante recibía un token POAP por su participación, luego cada token POAP hubo que verificarlo mediante un StorageProof, demostrando que eres el dueño del POAP y que el POAP pertenece al evento correspondiente. 
## getProof
Mi solución Solution/getPoapProof.ts fue crear un script de TypeScript mediante la biblioteca ethers.js que dada una wallet se interactuara con la red GNOSIS para obtener el balance (cantidad de tokens) de ella. Luego por cada token de la wallet de ser posible se obtenía el proof owner y proof event mediante el llamado a la función eth_getProof con los valores correspondientes.