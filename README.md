# its-me-the-one

struct Token 
    balances: HashMap<ActorId, u128>,
    allowances: HashMap<ActorId, HashMap<ActorId, u128>>,
    nonces: HashMap<ActorId, u64>,
    account_to_tx_ids: HashMap<ActorId, Vec<TxHash>,
    tx_ids: HashMap<TxHash, (TokenMessage, TxResult)>,
    deposits: HashMap<ActorId, u128>,
}