<br />
<div align="center">
<h3 align="center">LSTM network in modeling EGP-USD exchange rate</h3>

  <p align="center">
    Modeling EGP-USD currency exchange rate using LSTM neural networks with data containing USD, EUR, GBP exchange rates on Jupyter Notebook.
    <br />
    <a href="https://github.com/Mohamed-ElGemeie/LSTM-in-modeling-EGP-USD-exchange-rates/blob/main/Research%20paper.pdf"><strong>
    Research Paper</strong></a>
  </p>
</div>



<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      ![image](https://github.com/Mohamed-ElGemeie/LSTM-in-modeling-EGP-USD-exchange-rates/blob/main/assets/usd_pred_vs_usd.PNG?raw=true)
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#Contributors">Contributors</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
  </ol>
</details>



## About The Project

[![Product Name Screen Shot][product-screenshot]](https://example.com)


<p align="right">(<a href="#top">back to top</a>)</p>



### Built With

* [Python 3.9.7](https://www.python.org/downloads/release/python-397/)
* [Jupyter Notebook](https://jupyter.org/install)

<p align="right">(<a href="#top">back to top</a>)</p>



## Getting Started

The project runs through 4 phases each with their own dependencies and installments. 
<br>
- Phase 1 (Data Acquisition) 

    - Create a Google sheet with the data of the three currencies with the ```=GOOGLEFINANCE``` function.
    
    - Example: ```=GOOGLEFINANCE("CURRENCY:USDEGP","price",DATE(2003,1,12),DATE(2023,4,1),"DAILY")``` retrives the 1 USD to EGP exchange price from 2003/12/1 till 2023/4/1.
    
    - Do the same for the Euro and Great British pound, in the following columns. Check this [Google sheet](https://docs.google.com/spreadsheets/d/1gpDPDQSPgtsBQrfgfsSrwuzg1PQKyEZ589Go3H9nJ70/edit?usp=sharing) should look something like this: ![image]("https://github.com/Mohamed-ElGemeie/LSTM-in-modeling-EGP-USD-exchange-rates/blob/main/assets/Excel%20sheet%20example.PNG?raw=true") 

- Phase 2 (Data Retrieval) Easier Alternative
    - Simply download the sheet as a .csv file from a Google sheet (File >> download >> .csv).
    - Place the file in the Repo's folder named "data" and rename it as "USD-EGP Time series Data - raw.csv"
    
- Phase 2 (Data Retrieval) Harder Alternative

    - Enable the Google Workspace API to access this sheet through Python check [google developers doc](https://developers.google.com/sheets/api/quickstart/python) to get started.
    
    - Run the Notebook file [<b>Excel_sheet_importer</b>]() to get the sheet's data, and save it as a .csv file.
    
- Phase 3 (Data Cleaning)
    - Run the Notebook file [<b>Data_Cleaning</b>]() to clean the Dataset and export it as a .csv file.
- Phase 4 (Modeling)
    - Run the notebook [<b>USD-EGP Time series LSTM prediction</b>]() and tweak any hyperparameters if you wish.
    
    
### Prerequisites

The following dependencies need to be installed.
* pip
  ```sh
  pip install pandas
  pip install numpy
  pip install matplotlib
  pip install scikit-learn
  pip install keras
  
  // Google Workspace API
  pip install oauth2client
  pip install gspread

  ```
  

### Installation

* Download Tensorflow 2.0 and check [Tensorflow with pip](https://www.tensorflow.org/install/pip).


<p align="right">(<a href="#top">back to top</a>)</p>



## Usage
You can change the following in this project:
- Change the features.
- Change the testing and training data.
- Hyperparameters, Loss function.
- Use different model architectures.
<br><br>
Some changes must be accounted for throughout the whole program.
<br><br>
Also You can use the pretrained model in the folder [ModelG]()

<p align="right">(<a href="#top">back to top</a>)</p>




## Contributors

- Omar A. Morshdy [GitHub](https://github.com/Morshedy22)

- Ahmed K. Ahmed [GitHub](https://github.com/ahmed-shaapan)

- Nadeen M. Farid [GitHub](https://github.com/nadeenfarid)

- Mohamed G. ElGemeie [GitHub](https://github.com/Mohamed-ElGemeie) 

- Amira A. ElSharaby [Github](https://github.com/meroo12273)

- Omar M. Shehata []()

- Mohamed H. Abdrabou []()



## License

Distributed under the MIT License. See `LICENSE.txt` for more information.

<p align="right">(<a href="#top">back to top</a>)</p>



## Contact

Mohamed Elgemeie -- [Linkedin](https://www.linkedin.com/in/mohamed-elgemeie/) -- mgalal2002@outlook.com

Project Link: https://github.com/Mohamed-ElGemeie/LSTM-in-modeling-EGP-USD-exchange-rates




## Acknowledgments

* Thanks to our very kind and loving doctor Amira Mofreh Ibrahim, and our teaching assistant Amr Elsayed Elazazy

<p align="right">(<a href="#top">back to top</a>)</p>
