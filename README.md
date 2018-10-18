#TYDZIEN3.1
„Zbuduj prostą konwencję nazewniczą dla min. takich zasobów jak Grupa Zasobów, VNET, Maszyn Wirtualna, Dysk, Konta składowania danych. Pamiętaj o ograniczeniach w nazywaniu zasobów, które występują w Azure”

Wszystkie informacje o zasobie, które są identyfikowane przez metadane danego zasobu nie powinny być dublowane w jego nazwie. Np. lokalizacja, grupa zasobów, subskrypcja, itp.
Wszystkie zasoby muszą być otagowane: projekt, MPK, środowisko i inne wartości przydatne do np. analizy kosztów (max 15 tagów)


| Zasób | Nazwa | Liczba znaków |
| :---| :---|:---|
|Resource Group| `<service short name>-<environment>-rg` | 1-90|
|Virtual Network| `<context>-vnet` | 1-64|
|Subnet| `<descriptive context>`| 1-80
|Network Interface|`<vmname>-nic<num>`|1-80
|Public IP|`<vm or service name>-pip`|1-80
|NSG|`<context>-nsg`|1-80
|Virtual Machine| `<os>-<role>-vm<number>` |1–15 (Windows), 1–64 (Linux)|
|Disks| `<company><vm name without hyphens>st<number>` | 3-24
|Storage| `<company><service short name><environment>`| 3-24|
