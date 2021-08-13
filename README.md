# VPC - Creación de Snapshot 💻💾
<br />

## Índice  📰
1. [Pre-Requisitos](#Pre-Requisitos-pencil)
2. [Crear Snapshot](#Crear-Snapshot-ballot_box)
3. [Referencias](#Referencias-mag)
4. [Autores](#Autores-black_nib)
<br />


## Pre Requisitos :pencil:
* Contar con una cuenta en <a href="https://cloud.ibm.com/">IBM Cloud</a>.
* Contar con un grupo de recursos.
* Contar con una *VPC*.
* Contar con una *VSI* en *VPC*.

<br />

## Crear Snapshot :ballot_box:
Para crear un *Snapshot(instantánea)* de volumen de *Block Storage* para *VPC* realice los siguientes pasos:

1. En el ```Menú de navegación/Navigation menu``` seleccione la opción ```Infraestructura VPC/VPC Infrastructure```.

2. En la sección de ```Computación/Compute``` de click la pestaña ```Instancias de servidor virtual/Virtual server instances```. Posteriormente, seleccione la *VSI* en la cual desea trabajar. Tenga en cuenta la región en la que está su *VSI*.

3. Diríjase a la sección de ```Volúmenes de almacenamiento/Storage volumes``` y de click en el ```Volúmen de arranque/Boot volume``` de la *VSI*.

4. Seleccione la pestaña ```Instantáneas/Snapshots``` y de click en el botón ```Crear +/Create +```.

5. En la nueva ventana complete los campos sugeridos de la siguiente manera:
<br />

**Detalles/Details** 
* ```Nombre/Name```: indique un nombre exclusivo para su *Snapshot*.
* ```Grupo de recursos/Resource group```:
* ```Región/Region```:
<br />

**Volumen/Volume**
* Seleccione el volumen

<br />

<p align="center"><img width="700" src="https://github.com/emeloibmco/VPC-Creacion-Snapshot/blob/main/images/vpc-crear-snapshot.gif"></p>
<br />

## Referencias :mag:
* <a href="https://cloud.ibm.com/docs/vpc?topic=vpc-snapshots-vpc-create&interface=ui">Creating Snapshots</a>.
<br />

## Autores :black_nib:
Equipo *IBM Cloud Tech Sales Colombia*.
<br />
