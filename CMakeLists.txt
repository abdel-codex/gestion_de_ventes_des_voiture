
cmake_minimum_required(VERSION 3.10)
project(GestionVenteVoitures VERSION 1.0 LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

# Dossier des fichiers d'en-tête
include_directories(${CMAKE_CURRENT_SOURCE_DIR}/include)

# Déclaration des sources du projet
set(SOURCES
    src/main.cpp
    src/Voiture.cpp
    src/GestionnaireVentes.cpp
)

# Création de l'exécutable
add_executable(GestionVenteVoitures ${SOURCES})
