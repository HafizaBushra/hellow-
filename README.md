# hellow-
I am using Firebase Admin SDK for PHP v 7.2.28
Problem
Error: Call to private method Kreait\Firebase\ServiceAccount::fromJsonFile() from context

While trying to use some methods as follows;
$serviceAccount = ServiceAccount::fromJsonFile(DIR . '/firebase_credentials.json');
$firebase = (new Factory)
->withServiceAccount($serviceAccount)
->create();
I tried to edit fromJsonFile() from private to public and seemed like it worked then I landed to another issue, this method withServiceAccount does not exists
Error : Call to undefined method Kreait\Firebase\Factory::withServiceAccount()
