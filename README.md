# [EN] [Books to scrape](https://books.toscrape.com) scraping Python script

## Features
* Scrape books informations from the [Books to scrape](https://books.toscrape.com) website using BeautifulSoup4 and generate CSV files.

* Implement an object from **WebsiteScraper** class that scrapes the books categories and call a **CategoryScraper** for each found one.

* Implement an object from **CategoryScraper** class that scrape the books URLs for each category and call a **ProductScraper** for each found one.

* Implement an object from **ProductScraper** class that scrape informations from a product page, using an ETL (extract - transform - load) process :
    1. Extract the data from the page.    
    2. Transform the data so they fit the CSV file format.
    3. Write a CSV with following characteristics :
        1. Columns are the following (in this order) :
            * product_page_url,
            * universal_product_code,
            * title,
            * price_including_tax,
            * price_excluding_tax,
            * number_available,
            * product_description,
            * category,
            * review_rating,
            * image_url.
        2. Columns are separated by commas.
        3. Data record/line of fields (one by product) are separated by new lines.
        4. Fields are separated by commas.
        5. Fields are delimited by double-quotes (double-quotes inside fields are escaped by being replaced by two double-quotes).

* When running the main.py script, a terminal dialog let you chose the path where the CSV files will be created and ask to confirm it. Then it scrapes the whole website and create one directory (containing a CSV file and un directory with all the images of the category) by books category.

* The created CSV files can be opened with Libre Office Calc, Microsoft Office Excel or any CSV file reader/editor.

<br><br><br>
## Installation

### Download the source (and unzip it if needed)
Download the source code using one of the three following ways :
* Click on this [link](https://github.com/YaShuHee/OpenClassrooms_Project_2/archive/production.zip) and unzip the downloaded archive.
* From Github, click on "Code > Download ZIP" and unzip the downloaded archive.
* After installing [Git](https://git-scm.com/downloads), clone it with the command :
    ```shell script
    git clone https://github.com/YaShuHee/OpenClassrooms_Project_2
    ```

<br><br>
### Environment configuration

#### Install Python3
Install [Python3](https://www.python.org/downloads/) on your computer (version 3.8 or later).


#### Create a Python3 virtual environment
Run this command from inside the "OpenClassrooms_Project_2" directory you unzipped sooner :
* On Windows :
    ```shell script
    py -3 -m venv env
    ```

* On Linux/MacOS :
    ```shell script
    python3 -m venv env
    ```
It will create a directory named "env", including a full Python3 virtual environment, totally independant from your main Python3 installation, having its own installed packages.

* On Windows :
    You can now activate your virtual environment to use it (to execute code and to modify installed packages on it) by running the following command :
    ```shell script
    . .\env\Scripts\activate
    ```

* On Linux/MacOS :
    You can now activate your virtual environment to use it (to execute code and to modify installed packages on it) by running the following command :
    ```shell script
    . ./env/bin/activate
    ```
To exit the virtual environment without exiting your commandline, run this :
 ```shell script
deactivate
```

#### Install requirements
Activate the virtual environment you just installed with the previously mentionned command :
* On Windows
    ```shell script
    . .\env\Scripts\activate
    ```
* On Linux/MacOS :
    ```shell script
    . ./env/bin/activate
    ```
Now (still from the project root), run :
```shell script
pip install -r requirements.txt
```
Congratulations !
Your virtual environment is fully installed.
From now, whenever you want to run the project, just activate your environment and follow the [User instructions](#user-instructions).


<br><br><br>
## User instructions
Just run the main.py script with python, by running this command from the project 's root :
```shell script
python ./src/main.py
```

<br><br><br><br>
# [FR] Script Python de scraping du site [Books to scrape](https://books.toscrape.com)

## Fonctionnalit??s

* Scraping des informations du site [Books to scrape](https://books.toscrape.com) ?? l'aide de BeautifulSoup4 et g??n??ration de fichiers CSV.

* Impl??mentation d'un objet de la classe **WebsiteScraper** qui r??cup??re les cat??gories de livre et appelle un **CategoryScraper** pour chaque cat??gorie trouv??e.

* Impl??mentation d'un objet de la classe **CategoryScraper** qui r??cup??re les URL des livres de la cat??gorie et appelle un **ProductScraper** pour chaque livre trouv??.

* Impl??mentation d'un objet de la classe **ProductScraper** qui r??cup??re les informations d'une page produit, en utilisant un processus ETL (extract - transform - load) :
    1. Extraction des donn??es de la page.    
    2. Transformation et formatage des donn??es en vue de leur int??gration au fichier CSV. 
    3. Cr??ation d'un fichier CSV avec les caract??ristiques suivantes :
        1. Les colonnes sont les suivantes (dans cet ordre) :
            * product_page_url,
            * universal_product_code,
            * title,
            * price_including_tax,
            * price_excluding_tax,
            * number_available,
            * product_description,
            * category,
            * review_rating,
            * image_url.
        2. Les colonnes sont s??par??es par des virgules.
        3. Il n'y a qu'une ligne d'informations/champs (un seul produit).
        4. Les champs sont s??par??s par des virgules.
        5. Les champs sont d??limit??s par des guillemets (on escape les guillemets ?? l'int??rieur des champs en les doublant).

* ?? l'ex??cution du script main.py, le terminal demande interactivement le chemin vers le dossier dans lequel les fichiers CSV seront g??n??r??s, puis la confirmation de ce chemin. Ensuite, le site entier est scrap?? et un dossier (contenant un fichier CSV et un dossier avec toutes les images de la cat??gorie) est g??n??r?? par cat??gorie.

* Le fichier CSV cr???? peut ??tre ouvert ?? l'aide de Libre Office Calc, Microsoft Office Excel ou tout autre lecteur/??diteur de fichiers CSV.

<br><br><br>
## Installation

### T??l??chargez le code source (et d??compressez l'archive si n??cessaire)
T??l??chargez le code source en utilisant l'une des trois m??thodes suivantes :
* Cliquez sur ce lien [link](https://github.com/YaShuHee/OpenClassrooms_Project_2/archive/production.zip) et d??compressez l'archive t??l??charg??e.
* Depuis GitHub, cliquez sur "Code > Download ZIP" et d??compressez l'archive t??l??charg??e.
* Apr??s avoir install?? [Git](https://git-scm.com/downloads), clonez le code source ?? l'aide de la commande :
    ```shell script
    git clone https://github.com/YaShuHee/OpenClassrooms_Project_2
    ```

<br><br>
### Configuration de l'environnement

#### Installez Python3
Installez [Python3](https://www.python.org/downloads/) sur votre ordinateur (version 3.8 ou plus).

#### Cr??ez un environnement virtuel Python3
Ex??cutez cette commande depuis la racine du projet "OpenClassrooms_Project_2" que vous avez t??l??charg?? plus t??t :
* Sur Windows :
    ```shell script
    py -3 -m venv env
    ```

* Sur Linux/MacOS :
    ```shell script
    python3 -m venv env
    ```
Un dossier "env" est cr????, contenant un environnement virtuel Python3 totalement fonctionnel et ind??pendant de votre installation principale de Python3, avec ses propres packets install??s.

* Sur Windows :
    Vous pouvez d??sormais activer votre environnement virtuel (pour ex??cuter du code ou modifier les packets install??es) en ex??cutant la commande suivante :
    ```shell script
    . .\env\Scripts\activate
    ```

* Sur Linux/MacOS :
    Vous pouvez d??sormais activer votre environnement virtuel (pour ex??cuter du code ou modifier les packets install??es) en ex??cutant la commande suivante :
    ```shell script
    . ./env/bin/activate
    ```
Pour quitter l'environnement virtuel sans fermer le terminal, ex??cutez la commande suivante :
 ```shell script
deactivate
```

#### Installez les packets pr??requis
Activez l'environnement virtuel cr???? avec la commande mentionn??e pr??c??demment :
* Sur Windows
    ```shell script
    . .\env\Scripts\activate
    ```
* Sur Linux/MacOS :
    ```shell script
    . ./env/bin/activate
    ```
?? pr??sent (toujours depuis la racin du projet), ex??cutez :
```shell script
pip install -r requirements.txt
```
F??licitations !
Votre environnement virtuel est compl??tement install??.
D??sormais, d??s que vous voulez utiliser ce projet, activez simplement votre environnement virtuel et suivez le [Mode d'emploi](#mode-demploi).


<br><br><br>
## Mode d'emploi
Ex??cutez simplement le script main.py avec python en tapant la commande suivante depuis la racine du projet :
```shell script
python ./src/main.py
```