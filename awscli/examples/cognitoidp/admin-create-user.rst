**To create a user**

This example creates username diego@example.com. An email address and phone number
are specified. 

Command::

  aws cognito-idp admin-create-user --user-pool-id us-west-a_aaaaaaaaa --username diego@example.com --user-attributes=Name=email,Value=kermit2@somewhere.com,Name=phone_number,Value="+15555551212" --message-action SUPPRESS

Output::

  {
    "User": {
        "Username": "7325c1de-b05b-4f84-b321-9adc6e61f4a2",
        "Enabled": true,
        "UserStatus": "FORCE_CHANGE_PASSWORD",
        "UserCreateDate": 1548099495.428,
        "UserLastModifiedDate": 1548099495.428,
        "Attributes": [
            {
                "Name": "sub",
                "Value": "7325c1de-b05b-4f84-b321-9adc6e61f4a2"
            },
            {
                "Name": "phone_number",
                "Value": "+15555551212"
            },
            {
                "Name": "email",
                "Value": "diego@example.com"
            }
        ]
    }
  }
  
