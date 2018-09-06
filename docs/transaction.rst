===========
Transaction
===========
Sale
----
::

  <Req>
    <Cmd>
      <CmdId>TxnStart</CmdId>
    </Cmd>
    <Param>
      <Txn>
        <TxnType>Sale</TxnType>
        <AccType>Credit/Debit</AccType>
        <CurrCode>840</CurrCode>
        <TxnAmt>5.00</TxnAmt>
      </Txn>
    </Param>
  </Req>

Void
----
Cancel
------
::

  <Req>
    <Cmd>
      <CmdId>TxnCancel</CmdId>
    </Cmd>
  </Req>
