# WebAuthn / FIDO2 API Codelab

This folder contains the source code for the WebAuthn / FIDO2 API codelab. It gives an introduction into implementing FIDO2 API,

- https://codelabs.developers.google.com/codelabs/fido2-for-android/

## Notes from Sharif

I started working through the Google Codelab linked above, but ran into an issue:

- running the project locally was causing some errors with the Webauthn code
  - resolved by using `localhost` instead of `localhost:8080` in the Express routes
- follow the steps in the _Get Started_ section below to enable the app to work properly

## Get Started

- `npm install`
- create an `.env` file in the root of the project with the following

```bash
PROJECT_NAME="passkeys codelab"
ENVIRONMENT="development"
HOSTNAME=""
ORIGIN=""
RP_NAME=""
```

- create a `.data` folder in the root of the project
- add an empty file `db.json.tmp` to the `.data` folder

- `npm start`
- navigate to http://localhost:8080/
- create a user by entering any username (no spaces or special characters)
- press "Next"
- press "Sign-In" to accept the pre-populated password
- press the "Create a Passkey" button
- authenticate with your local device
- press "Sign Out"
- back on the home screen, click into the "username" field
- select "Use a passkey" from the autofill
- select the username you just registered with
- authenticate with your local device again to access the passkey

### License

```
Copyright 2019 Google, Inc.

Licensed to the Apache Software Foundation (ASF) under one or more contributor
license agreements. See the NOTICE file distributed with this work for
additional information regarding copyright ownership. The ASF licenses this
file to you under the Apache License, Version 2.0 (the "License"); you may not
use this file except in compliance with the License. You may obtain a copy of
the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
License for the specific language governing permissions and limitations under
the License.
```
