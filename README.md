# basetyu
Detecting Wallets That Always Transact at the Same Gas Price
gas_prices = {tx["gasPrice"] for tx in wallet_txs}

if len(gas_prices) == 1 and len(wallet_txs) > 3:
    print("Static gas price wallet:", wallet)
