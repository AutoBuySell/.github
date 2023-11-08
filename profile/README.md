# AutoTrading project
Please follow the instructions below to get an automated trading service on your local environment.
## Installation
1. Make a project folder on your local machine
    1. **Windows10** and **MacOS Ventura** have been proved to be acceptable OSs
2. Following 3 repositories below should be placed in the project folder
    1. [Frontend server](https://github.com/AutoBuySell/AT_V0) which controls the other servers and shows the result logs
    2. [Backend server](https://github.com/AutoBuySell/Backend_server) which processes the overall services requested
    3. [Data server](https://github.com/AutoBuySell/Data_server) which mainly requests and processes data
3. One additional folder with subfolders should be placed in the project folder
    1. /data/
        1. /log_data/
        2. /market_data/
        3. /market_long_data/
        4. /setting_data/
        5. target_company.csv
            ```shell
            Symbol,Name,Judge
            TSLA,Tesla,1
            MSFT,Microsoft,1
            META,Meta platforms,1
            NVDA,Nvidia,1
            ```
    2. The subfolders above are free to be remain empty
4. Run 3 servers by following instructions
    1. [Frontend server](https://github.com/AutoBuySell/AT_V0)
    2. [Backend server](https://github.com/AutoBuySell/Backend_server)
    3. [Data server](https://github.com/AutoBuySell/Data_server)
5. Final folder structures
    ```shell
    Project folder
    ├── AT_V0
    │   ├── app
    │   ├── components
    │   ├── config
    │   └── ...
    ├── Backend_server
    │   ├── apis
    │   ├── apps
    │   ├── configs
    │   ├── main.py
    │   └── ...
    ├── Data_server
    │   ├── apis
    │   ├── apps
    │   ├── main.py
    │   └── ...
    └── data
        ├── log_data
        ├── market_data
        ├── market_long_data
        ├── setting_data
        └── target_company.csv
    ```
