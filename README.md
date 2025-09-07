# CLI Password Manager

A simple and secure **command-line password manager** built with Node.js.  
Store, retrieve, edit, and manage your platform passwords locally on your machine.

[![npm version](https://img.shields.io/npm/v/cli-password-manager?color=green&label=npm)](https://www.npmjs.com/package/cli-password-manager)

---

## Features

- Register a single user per machine
- Secure login with a master password
- Add, retrieve, edit, and list passwords for multiple platforms
- Delete account securely (requires system username + master password)
- Passwords are **encrypted locally** using AES-256-CTR
- Persistent login session

---

## Installation

```bash
npm install -g cli-password-manager
```
### To use the Package : 
```bash
 clim

```
### To Open Help Page 
```bash
 clim --help

```
### To Register a User  
```bash
 clim register <username>

```
### To Login a User
```bash
 clim login <username>
```
You will be asked to enter your password.

### Add Platform Password 
```bash
 clim add <platform> <username>
```
 Example : 
 ```bash
  clim add github mygithubuser

```
### Retrieve a Password
```bash
 clim get <platform>

```
### List all Stored Password 
```bash
 clim list

```
### Edit a Platform Password
```bash
 clim edit <platform>

```
### Logout 
```bash
 clim logout

```
### Delete User (in case you forgot password : Warning : All passwrods will be deleted.)
```bash
 clim delete <username>

```
## Storage
Passwords are stored locally at:
```bash
 ~/.cli-password-manager/db.json
```
Session details are stored at:
```bash
 ~/.cli-password-manager/session.json

```
## Security
Passwords are encrypted using AES-256-CTR.
Master password is hashed using bcryptjs.
All data is stored locally on your machine; no cloud storage.

## CLI Commands Overview

| Command                          | Description                                           |
|----------------------------------|-------------------------------------------------------|
| `clim register <username>`        | Register a new user                                   |
| `clim login <username>`           | Login to an existing user                             |
| `clim add <platform> <username>`  | Add a password entry for a platform                  |
| `clim get <platform>`             | Retrieve password for a platform                     |
| `clim list`                       | List all stored platforms                             |
| `clim edit <platform>`            | Edit password for a platform                          |
| `clim logout`                     | Logout of the current session                         |
| `clim delete <username>`          | Delete your account permanently (requires confirmation) |


Thanks 
~ Galactico 






