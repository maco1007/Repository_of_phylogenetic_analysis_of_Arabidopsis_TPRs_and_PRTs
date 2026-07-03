Repository of phylogenetic analysis of Arabidopsis TPRs and PRTs
Repository of phylogenetic analysis of Arabidopsis TPRs and PRTs

Análisis Filogenético con IQ-TREE: Familias de proteínas TPR
Este repositorio contiene los datos de entrada y los resultados de salida de una inferencia filogenética por Máxima Verosimilitud (Maximum Likelihood) realizada con el software IQ-TREE. El análisis se realizó a partir de un alineamiento múltiple de secuencias de proteínas que contienen repeticiones TPR (Tetratricopeptide repeats).

Detalles del Análisis
Programa: IQ-TREE versión 3.1.2

Comando ejecutado: iqtree -s mafft_TPRs_v3.1.fas -m MFP -bb 1000 -nt AUTO

Datos de entrada: Alineamiento de proteínas en formato FASTA.

Dimensiones del alineamiento: 74 secuencias y 1397 columnas (1223 patrones distintos, 815 sitios informativos para parsimonia).

Selección de Modelo: ModelFinder Plus (-m MFP). Evaluó múltiples modelos para encontrar el mejor ajuste evolutivo (por ejemplo, Q.PLANT+I+G4).

Prueba de Soporte: Ultrafast Bootstrap con 1000 réplicas (-bb 1000).

Índice de Archivos
A continuación se describe el propósito de cada archivo generado y almacenado en este repositorio:

Datos de Entrada
mafft_TPRs_v3.1.fas: Archivo de alineamiento múltiple original en formato FASTA generado por MAFFT.

Resultados Principales (Árboles)
mafft_TPRs_v3.1.fas.treefile: Árbol filogenético de Máxima Verosimilitud final en formato Newick. Este es el archivo principal que debes usar para visualizar el árbol topológico con las longitudes de las ramas originales.

mafft_TPRs_v3.1.fas.contree: Árbol de consenso construido a partir de las réplicas de bootstrap. Muestra los valores de soporte en los nodos.

Reportes e Información de la Corrida
mafft_TPRs_v3.1.fas.iqtree: Reporte principal y amigable para lectura humana. Contiene un resumen del análisis, el modelo evolutivo seleccionado, una representación del árbol en texto plano y los parámetros de las tasas de sustitución.

mafft_TPRs_v3.1.fas.log: Registro completo (log) de todo el proceso de IQ-TREE por la terminal. Útil para depurar o revisar los tiempos de cómputo y la convergencia de la búsqueda.

Archivos Secundarios / Datos Intermedios
mafft_TPRs_v3.1.fas.bionj: Árbol inicial construido mediante el método Neighbor-Joining (BIONJ), el cual sirvió como punto de partida para la optimización de Máxima Verosimilitud.

mafft_TPRs_v3.1.fas.mldist: Matriz que contiene las distancias genéticas de pares estimadas por Máxima Verosimilitud.

mafft_TPRs_v3.1.fas.splits.nex: Archivo en formato NEXUS que contiene la información de las particiones (splits) de los árboles de bootstrap.

mafft_TPRs_v3.1.fas.model.gz: Archivo comprimido con un registro detallado de los log-likelihoods de todos los modelos evolutivos probados durante la fase de ModelFinder.

mafft_TPRs_v3.1.fas.ckp.gz: Archivo de punto de control (checkpoint). Permite reanudar el análisis desde donde se quedó en caso de que hubiera sido interrumpido.

Cómo visualizar los resultados
Para visualizar los archivos de los árboles (.treefile o .contree), puedes descargar los archivos y abrirlos con cualquier visualizador de árboles filogenéticos estándar, como:

FigTree (Escritorio)

iTOL - Interactive Tree Of Life (Web)

Dendroscope (Escritorio)
