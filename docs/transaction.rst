===========
Transaction
===========
Sale
----
Request
"""""""
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
Response
""""""""

-----------------------------------

Void
----
Request
"""""""
::

  <Req>
    <Cmd>
      <CmdId>TxnStart</CmdId>
    </Cmd>
    <Param>
      <Txn>
        <TxnType>Void</TxnType>
        <TxnId>${TxnId}</TxnId>
      </Txn>
    </Param>
  </Req>
Response
""""""""

-----------------------------------

Cancel
------
Request
"""""""
::

  <Req>
    <Cmd>
      <CmdId>TxnCancel</CmdId>
    </Cmd>
  </Req>
Response
""""""""
::

  <Resp>
    <Cmd>
      <CmdId>TxnCancelResp</CmdId>
      <StatusCode>0000</StatusCode>
      <StatusText>Successful</StatusText>
    </Cmd>
  </Resp>

-----------------------------------
