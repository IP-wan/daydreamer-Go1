# daydreamer-Go1

### 1. Устанавливаем систему управления пакетами conda
### 2. Клонируем репозиторий с github
```
git@github.com:IP-wan/daydreamer-Go1.git
```
### 3. Переходим в директорию
```
cd daydreamer-Go1
```
### 4. Создаем виртуальное окружение
```
conda create -n <name env>
```
### 5. Активируем виртуальное окружение
```
conda activate <name env>
```
### 6. Устанавливаем версию python
```
conda install python==3.10
```
### 7. Устанавливаем зависимости из файла requirements
```
pip install -r requirements.txt 
```
### 8. Создаем файл sdk
#### 8.1 Переходим в директорию
```
cd third_party/unitree_legged_sdk/
```
#### 8.2 Выполняем команды
```
mkdir build
cd build
cmake ..
make
```
#### 8.3 Файл из директории build robot_interface.cpython-310-x86_64-linux-gnu.so копируем в /motion_imitation/