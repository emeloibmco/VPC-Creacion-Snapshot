# VPC - Creación de Snapshot 💻💾
*Snapshots for VCP* (instantáneas para *VPC*) son una oferta regional que se utiliza para crear una copia puntual de su volumen de datos o arranque de almacenamiento en bloque. La instantánea inicial que toma es una copia de seguridad completa del volumen. Las instantáneas posteriores del mismo volumen son incrementales; solo se capturan los cambios desde las últimas instantáneas. Puede seleccionar una instantánea durante el aprovisionamiento de la instancia y restaurar un nuevo volumen de arranque completamente aprovisionado para iniciar la instancia. También puede crear y adjuntar un volumen de datos a partir de una instantánea dentro de una instancia de servidor virtual en ejecución.

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
Para crear un *Snapshot (instantánea)* del volumen de arranque de *Block Storage* para *VPC* siga los pasos que se muestran a continuación:

1. En el ```Menú de navegación/Navigation menu``` seleccione la opción ```Infraestructura VPC/VPC Infrastructure```.

2. En la sección de ```Computación/Compute``` de click la pestaña ```Instancias de servidor virtual/Virtual server instances```. Posteriormente, seleccione la *VSI* en la cual desea trabajar. Tenga en cuenta la región en la que está su *VSI*.

3. Diríjase a la sección de ```Volúmenes de almacenamiento/Storage volumes``` y de click en el ```Volúmen de arranque/Boot volume``` de la *VSI*.

4. Seleccione la pestaña ```Instantáneas/Snapshots``` y de click en el botón ```Crear +/Create +```.

5. En la nueva ventana complete los campos sugeridos de la siguiente manera:
<br />

**Detalles/Details** 
* ```Nombre/Name```: asigne un nombre exclusivo para su *Snapshot*.
* ```Grupo de recursos/Resource group```: seleccione el grupo de recursos en el cual está trabajando.
* ```Región/Region```: indique la región en donde está trabajando.
<br />

**Volumen/Volume**
* Seleccione el volumen de almacenamiento sobre el que quiere crear el *Snapshot*.
<br />

6. De click en el botón ```Crear instantánea/Creat snapshot``` y espere unos minutos mientra se completa la solicitud para la creación del *Snapshot*.

7. Refresque la sección de los *Snapshots* con la opción 🔄 y espere mientra se completa el proceso.

<br />

<p align="center"><img width="700" src="https://github.com/emeloibmco/VPC-Creacion-Snapshot/blob/main/images/vpc-crear-snapshot.gif"></p>
<br />

## Referencias :mag:
* <a href="https://cloud.ibm.com/docs/vpc?topic=vpc-snapshots-vpc-create&interface=ui">Creating Snapshots</a>.
* <a href="https://cloud.ibm.com/docs/vpc?topic=vpc-snapshots-vpc-about">About Snapshots for VPC</a>.
<br />

## Autores :black_nib:
Equipo *IBM Cloud Tech Sales Colombia*.
<br />
