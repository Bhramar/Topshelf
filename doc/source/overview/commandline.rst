Topshelf Command-Line Reference
"""""""""""""""""""""""""""""""

Once a service has been created using Topshelf, an extensive command-line vocabulary is available which can be used to install, uninstall, start, and configure the service.

The command-line help can be displayed at any time by entering ``myService.exe help`` on the command-line.

Help Text
'''''''''

The help text from the command line is shown below for easy reference.


    service.exe **[verb]** [-option:value] [-switch]

    **run**               Runs the service from the command line (default)
    
    **help** or **--help**      Displays help

    **install**           Installs the service

      -username         The username to run the service
      -password         The password for the specified username
      -instance         An instance name if registering the service
                        multiple times
      --autostart       The service should start automatically (default)
      --disabled        The service should be set to disabled
      --manual          The service should be started manually
      --delayed         The service should start automatically (delayed)
      --localservice    Run the service with the local service account
      --networkservice  Run the service with the network service permission
      --interactive     The service will prompt the user at installation for
                        the service credentials
      --sudo            Prompts for UAC if running on Vista/W7/2008

      -servicename      The name that the service should use when
                        installing
      -description      The service description the service should use when
                        installing
      -displayname      The display name the the service should use when
                        installing

    **start**             Starts the service if it is not already running

      -instance           The instance to start

    **stop**              Stops the service if it is running

      -instance           The instance to stop

    **uninstall**         Uninstalls the service

      -instance         An instance name if registering the service
                        multiple times
      --sudo            Prompts for UAC if running on Vista/W7/2008
