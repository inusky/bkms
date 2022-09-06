- working on cloudshell with root login
  stech
  aws route53domains transfer-domain-to-another-aws-account --domain-name skyinnk.com --account-id Account ID sel --region us-east-1
- Account id of receiver

{
"OperationId": "c4446330-dd34-4e72-bb4c-88458a8e2a71",
"Password": "IHECQ*2(w8R6*X"
}

- working on cloudshell with root login
  sel
  aws route53domains accept-domain-transfer-from-another-aws-account --domain-name skyinnk.com --password "IHECQ*2(w8R6*X" --region us-east-1

{
"OperationId": "fa680f52-8ab7-4197-b9e9-5725d7ef5d7f"
}

aws route53domains cancel-domain-transfer-to-another-aws-account --domain-name skyinnk.com

=======================================================================================

# Initiate Domain Transfer

aws route53domains transfer-domain-to-another-aws-account --domain-name yourdomain.tld --account-id 123456789101

# Cancel Domain Transfer

aws route53domains cancel-domain-transfer-to-another-aws-account --domain-name yourdomain.tld
{
"OperationId": "MNOP-MNOP-MNOP-MNOP-MNOP",
"Password": "XYZXYZXYZXYZ"
}

# Accept Domain Transfer

aws route53domains accept-domain-transfer-from-another-aws-account --domain-name yourdomain.tld --password "XYZXYZXYZXYZ"
