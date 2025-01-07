makefile
TARGET=guessinggame.sh

all: README.md

README.md: $(TARGET)
	echo "# Projet Guessing Game" > README.md
	echo "" >> README.md
	echo "### Exécuté le : $$(date)" >> README.md
	echo "" >> README.md
	echo "### Nombre de lignes de code dans $(TARGET) : $$(wc -l < $(TARGET))" >> README.md
