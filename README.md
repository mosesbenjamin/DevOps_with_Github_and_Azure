#### To demo an extrenal trigger

    - Modify "on" property and specify repository_dispatch and type
    - Make a "POST" call to https://api.github.com/repos/owner/repo/dispatches
    - Set "Accept" header to "application/vnd.github.v3+json"
    - Set the body of the request:
       {
        "event_type": "run_my_workflow",
        "client_payload": {
            "mydata": "Some External Value"
        }
    }
