# gitctl

```
                            @@              
                          @...@             
                           @@@%%%@@@        
           %%%                /@@..@@\      
         @%@\       .%%%%%%%%%%%@@@%%@@\    
        .%@%%     /@.PushIt...%@/   .@%%@\  
        |%@%%    |@..PullIt...@|    .%@%/\  
        |(@%@    |@...BopIt...@|     @@@/|  
        |/%@%@    \@....../%%@/     .@@..|  
         \/&@#@@@@/..._@@@@@@/      /@../   
          \((@@%%%%%%/             /////    
           \%%%%@@@@@@             |//      
            \%%%%%%@@@                      
              \%%%%%@                       

```

## ABOUT

    A simple git wrapper for basic local project operations

    By default, all printed or suppressed verbosity messages are logged to
    local log files located in logs/ (relative to the location of the gitctl
    script). This logging feature can be disabled (see the "USAGE" section).

## USAGE

    hw_git <OPTION>
    hw_git <OPTION> <OPERATION>

    where "OPTION" is one or more of the following:

                  |
    -d, --dump    | Dump the contents of all gitctl log files to the standard
                  | output (overrides any specified "OPERATION" parameters)
                  |
    -f, --find    | Try to find a local project root directory and print
                  | the result to the standard output (overrides any
                  | specified "OPERATION" parameters)
                  |
    -h, --help    | Print this help text to the terminal (overrides
                  | verbosity and logging)
                  |
    -l, --log     | Log all verbosity messages (default)
                  |
    -n, --no-log  | Avoid writing verbosity messages to a log file
                  |
    -p "X",       |
    --project="X" | Set the repository project directory to "X"; where "X"
                  | is the absolute path to a local project git repository
                  | (if not specified, gitctl will attempt to discover
                  | where the project is located)
                  |
                  | NOTE: You may need to wrap X in quotes if your directory
                  | path contains spaces
                  |
    -s, --silent  | Suppress verbosity messages
                  |
    -v, --verbose | Display verbosity messages (default)
                  |

    and where "OPERATION" is one of the following:

                  |
    --bop "X",    |
    --bopit "X"   | Stage all changes and subsequently push all staged
                  | changes to the remote repository (combines both the
                  | '--stage' and '--push' operations); This operation
                  | may include an optional commit message, "X"
                  |
    --check,      |
    --checkit     | Check the status of the remote repository as compared
                  | with the local one
                  |
    --pull,       |
    --pullit      | Pull the latest version of the remote repository
                  |
    --push,       |
    --pushit      | Push new updates to the remote repository (requires
                  | previous execution of '--stage')
                  |
    --stage "X",  |
    --stageit "X" | Stage all modified, deleted, and new files (this is a
                  | required step before urnning '--push'); May include
                  | an optional commit message, "X"
                  |

## REFERENCE

<i>How to check the differences between local and github  (stackoverflow.com)</i>

https://stackoverflow.com/a/6000939

<i>Staging all changes (stackoverflow.com)</i>

https://stackoverflow.com/a/26982422

## ATTRIBUTION & LICENSE

    Created by h8rt3rmin8r (161803398@email.tg) on 20200827

    Copyright 2020 [Novx.ai](https://novx.ai/)

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.

