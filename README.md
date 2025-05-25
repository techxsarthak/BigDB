<div align="center">
<h1><kbd>🧩 BigDB</kbd></h1>
An extension for MIT App Inventor 2.<br>
BigDB - Advanced key-value storage with TTL, metadata, multi-table support, encryption, and more <br> <a href="https://ai2.sarthakdev.in">My Other Extensions</a> <br> Built by <a href="www.sarthakdev.in"> Sarthak Gupta</a>
</div>

## 📝 Specifications
📦 **Package:** com.bigdb
💾 **Size:** 33.66 KB
⚙️ **Version:** 1.0
📱 **Minimum API Level:** 7
📅 **Updated On:** [date=2025-05-25 timezone="Asia/Calcutta"]
💻 **Built & documented using:** [FAST-CLI](https://community.appinventor.mit.edu/t/fast-an-efficient-way-to-build-extensions/129103?u=jewel) `v2.8.1`

## <kbd>Events:</kbd>
**BigDB** has total 4 events.

### 💛 Got
Fires when a value is retrieved

| Parameter | Type
| - | - |
| queryId | text
| value | text

### 💛 KeyList
Fires when a key list is returned

| Parameter | Type
| - | - |
| queryId | text
| keys | any

### 💛 DataChanged
Fires when data changes in the current table

### 💛 ErrorOccurred
Fires when an error occurs

| Parameter | Type
| - | - |
| message | text

## <kbd>Methods:</kbd>
**BigDB** has total 28 methods.

### 💜 SetPassword
Set database encryption password (PRAGMA key)

| Parameter | Type
| - | - |
| pwd | text

### 💜 RemovePassword
Remove encryption (PRAGMA rekey to empty)

### 💜 IsEncrypted
Check if database is encrypted

### 💜 Store
Store a value for a key with optional TTL and metadata

| Parameter | Type
| - | - |
| key | text
| value | text
| useTTL | boolean
| ttlSeconds | number
| metadata | text

### 💜 Get
Get the value for a key asynchronously

| Parameter | Type
| - | - |
| key | text
| queryId | text

### 💜 Delete
Delete a key

| Parameter | Type
| - | - |
| key | text

### 💜 Clear
Clear all data in the current table

### 💜 RenameKey
Rename a key

| Parameter | Type
| - | - |
| oldKey | text
| newKey | text

### 💜 BulkStore
Store multiple key-value pairs

| Parameter | Type
| - | - |
| keys | list
| values | list

### 💜 BulkDelete
Delete multiple keys

| Parameter | Type
| - | - |
| keys | list

### 💜 Keys
List all keys in the current table asynchronously

| Parameter | Type
| - | - |
| queryId | text

### 💜 Exists
Check if a key exists

| Parameter | Type
| - | - |
| key | text

### 💜 GetRecord
Get full record as JSON asynchronously

| Parameter | Type
| - | - |
| key | text
| queryId | text

### 💜 FindByMetadata
Find keys by metadata substring asynchronously

| Parameter | Type
| - | - |
| query | text
| queryId | text

### 💜 Expire
Set expiry time in seconds for a key

| Parameter | Type
| - | - |
| key | text
| seconds | number

### 💜 SetMetadata
Set metadata for a key

| Parameter | Type
| - | - |
| key | text
| metadata | text

### 💜 GetMetadata
Get metadata for a key

| Parameter | Type
| - | - |
| key | text

### 💜 GetTTL
Get remaining TTL in seconds for a key (0 if none or expired)

| Parameter | Type
| - | - |
| key | text

### 💜 PurgeExpired
Purge expired keys from the current table

### 💜 ExportCSV
Export current table as CSV to the specified file path. If filePath is empty, uses the app's external files directory.

| Parameter | Type
| - | - |
| filePath | text

### 💜 ImportCSV
Import data into current table from CSV

| Parameter | Type
| - | - |
| filename | text

### 💜 ExportJSON
Export current table as JSON string

### 💜 ImportJSON
Import data into current table from JSON

| Parameter | Type
| - | - |
| json | text

### 💜 Count
Get total record count in current table

### 💜 DBSize
Get database file size in bytes

### 💜 ListTables
List all tables in database

### 💜 Watch
Watch changes to a key in the current table

| Parameter | Type
| - | - |
| key | text
| queryId | text

### 💜 Unwatch
Stop watching changes to a key

| Parameter | Type
| - | - |
| key | text
| queryId | text

## <kbd>Setter:</kbd>
**BigDB** has total 1 setter property.

### 💚 SetTable
Set the current table to operate on

* Input type: `text`

