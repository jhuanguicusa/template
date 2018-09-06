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
::

  <Resp>
    <Cmd>
      <CmdId>TxnStartResp</CmdId>
      <StatusCode>0000</StatusCode>
      <StatusText>Successful</StatusText>
    </Cmd>
    <Data>
      <Txn>
        <TxnResult>02</TxnResult>
        <TxnResultMsg>Online Approved</TxnResultMsg>
        <TxnId>1102037634</TxnId>
        <RspCode>00</RspCode>
        <RspText>APPROVAL</RspText>
        <CardType>Visa</CardType>
        <AuthCode>VI0500</AuthCode>
        <PAN>4761530000001118</PAN>
        <TxnAmt>5.00</TxnAmt>
      </Txn>
    </Data>
  </Resp>
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
