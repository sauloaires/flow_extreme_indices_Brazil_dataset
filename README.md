# flow_extreme_indices_Brazil_dataset

This dataset readme file was created by Dirceu Silveira Reis Junior on 2022-05-07.

### General information

1. Title of Dataset : Data from: Trend detection in annual streamflow extremes in Brazil

2. Author Information

- Principal Investigator Contact Information

        Name: Saulo Aires de Souza
        Institution: Agência Nacional de Águas e Saneamento Básico
        Address:  Brasilia DF #####-###, Brazil
        Email: saulo.souza@ana.gov.br or sauloaires@gmail.com
           
- Associate or Co-investigator Contact Information

        Name: Dirceu Silveira Reis Junior
        Institution: University of Brasilia
        Address: Campus Darcy Ribeiro, Dept. de Engenharia Civil e Ambiental, Brasilia DF 70910.900, Brazil
        Email: dirceureis@unb.br or dirceu.reis@gmail.com 


3. Date of data collection (single date, range, approximate date) <suggested format YYYYMMDD> N/A

4. Geographic location of data collection (where was data collected?): N/A

5. Information about funding sources that supported the collection of the data: 

- Coordenação de Aperfeiçoamento de Pessoal de Nível Superior -Brazil (CAPES), finance code 001, Brazilian National Water Agency (ANA), Edital Mudanças Climáticas e Recursos Hídricos No. 19/2015.

- Conselho Nacional de Desenvolvimento Científico e Tecnológico (CNPq), CHAMADA UNIVERSAL MCTI/CNPq Nº 01/2016.


--------------------------
SHARING/ACCESS INFORMATION
-------------------------- 

1. Licenses/restrictions placed on the data:  CC0 1.0 Universal (CC0 1.0) Public Domain Dedication  (https://creativecommons.org/publicdomain/zero/1.0/)

2. Links to publications that cite or use the data:  to be defined after review processs.

3. Links to other publicly accessible locations of the data: N/A

4. Links/relationships to ancillary data sets: N/A

5. Was data derived from another source? No

6. Recommended citation for the data: Souza, Saulo A., Reis, Dirceu S Jr (2022) Data from: Trend detection in annual streamflow extremes in Brazil [Dataset]. GitHub Repository. (doi number to be defined)

---------------------
DATA & FILE OVERVIEW
---------------------

1. File List      

The dataset contains 8 folders, one for each of the following flow indices: 

- QX1d:	Annual maximum daily flow
- QX5d:	Annual maximum 5-day consecutive average flow
- QX30d:	Annual maximum 30-day consecutive average flow
- Qmean	Mean annual streamflow
- Q7	Annual minimum 7-day consecutive average flow
- Q30	Annual minimum 30-day consecutive average flow
- Q7Wtri	Annual minimum 7-day consecutive average flow (wettest trimester)
- Q7Wsem	Annual minimum 7-day consecutive average flow (wettest semester)

Each folder contains 12 files, one for each hydrographic region: East Atlantic (ALE), Amazon (AMZ), Western Northeast Atlantic (ANC), Eastern North-east Atlantic (ANO), Southeast Atlantic (ASD), Southeast Atlantic (ATS), Parnaíba (PNB), Paraguai (PRG), Paraná (PRN), São Francisco (SFR), Tocantins-Araguaia (TOA), and Uruguai (URU), as shown below for the folder named "flow_index" 

- Files contained in the folder named "flow_index"
  - flow_index_RH ALE.dat
  - flow_index_RH AMZ.dat
  - flow_index_RH ANC.dat
  - flow_index_RH ANO.dat
  - flow_index_RH ASD.dat
  - flow_index_RH ATS.dat
  - flow_index_RH PNB.dat
  - flow_index_RH PRG.dat
  - flow_index_RH PRN.dat
  - flow_index_RH SFR.dat
  - flow_index_RH TOA.dat
  - flow_index_RH URU.dat
  
2. Relationship between files: N/A

3. Additional related data collected that was not included in the current data package: N/A

4. Are there multiple versions of the dataset? No


### DATA-SPECIFIC INFORMATION FOR the .dat files

1. delimiter: semicolon

2. Rows (1-15) contain the following general information:

- BaciaCodigo: code of the river basin
- SubBaciaCodigo: code of the river sub-basin
- Estacao_codigo: code of the gauge
- Latitude
- Longitude
- Altitude
- AreaDrenagem: drainage area in km2.
- OrigemSerie: ? (Saulo)
- DescricaoOrigemSerie: type of flow index (Saulo, acho que está errao no arquivo)
- DiscretizaçãoTemporária: time scale. In this case, all series contain annaul values (A)
- TipodeDado: type of flow index
- MesAnoHidro: ? (Saulo)
- NomeEstacao: name of the gauge
- NomedoRio: name of the river
- Municipio: name of the municipality

3. The remaining rows contain the year and the value of the flow index for that year. There are two columns for each gauge. Therefore, the total number of columns is always twice the number of gauges.

4. "null" means there is no information for that year.


5. The number of rows and columns vary depending on the flow index and the hydrographic region.

6. All values of flow indeces are preseted in m3/s.

