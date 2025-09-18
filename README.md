# 🧠 Splunk Mind Map – Commands & Event IDs

```mermaid
mindmap
  root((Splunk))
    Usage
      Search
        index=main
        sourcetype=WinEventLog:Security
        host=PC-001
        source="WinEventLog:Security"
      Operators
        AND : All conditions must be true
        OR : At least one condition must be true
        NOT : Exclude a term or value
        pipe (|) : Chain multiple commands
    Commands
      stats : Aggregate and calculate values
        count : Total number of events
        avg : Average of a numeric field
        max : Maximum value
        min : Minimum value
      table : Create a table with specific columns
      sort : Sort results (asc/desc)
      top : Show the most frequent values
      rare : Show the least frequent values
      rex : Extract patterns using Regex
      fields : Include or exclude specific fields
    Windows Event ID
      Authentication
        4624 : Successful logon (user login succeeded)
        4625 : Failed logon (invalid password/account)
        4634 : Logoff (user signed out)
        4647 : User-initiated logoff
        4672 : Special privileges assigned to new logon
      User Accounts
        4720 : New user account created
        4722 : User account enabled
        4723 : Password change attempt
        4724 : Password reset attempt
        4725 : User account disabled
        4726 : User account deleted
        4732 : User added to a group
        4733 : User removed from a group
      Processes & Applications
        4688 : New process created
        4689 : Process exited
        4697 : New serv
