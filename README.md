# Instalacja

Wymagania:

* Anaconda

### Stworzenie środowiska

Komendy należy wykonać w wierszu poleceń Anaconda (Anaconda Prompt lub Anaconda Powershell Prompt), w katalogu repozytorium:

    conda create -y --name urszula_tomana python=3.8
    conda install -y --name urszula_tomana -c conda-forge --file requirements.txt

# Aktywacja środowiska i uruchomienie notebooka

    conda activate urszula_tomana
    jupyter notebook

# Formatowanie kodu

Dla zwiększenia czytelności i spójności kodu zaleca się wykorzystanie autoformattera `black` w formie rozszerzenia do jupyter notebook:

    jupyter nbextension install https://github.com/drillan/jupyter-black/archive/master.zip
    jupyter nbextension enable jupyter-black-master/jupyter-black

Do sortowania importów w obrębie komórek zaleca się skorzystanie z rozszerzenia `isort`:

    jupyter nbextension install https://github.com/benjaminabel/jupyter-isort/archive/master.zip
    jupyter nbextension enable jupyter-isort-master/jupyter-isort

# Usuwanie środowiska

Aby usunąć środowisko z komputera należy wykonać komendy:

    conda deactivate
    conda env remove -n urszula_tomana