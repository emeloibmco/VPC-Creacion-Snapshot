# VPC - Creación de Snapshot 💻💾
*Snapshots for VCP* (instantáneas para *VPC*) son una oferta regional de *IBM Cloud* que se utiliza para crear una copia puntual de un volumen de datos o de arranque. Para crear un *Snapshot*, el volumen original debe estar adjunto a una instancia de servidor virtual (*VSI*) en ejecución. El primer *Snapshot* es una copia de seguridad completa del volumen, mientras que los *Snapshots* posteriores del mismo volumen, registran solo los cambios desde la última instantánea creada. Puede utilizar un *Snapshot* de un volumen de arranque para aprovisionar una instancia. Por otro lado, si el *Snapshot* es de un volumen de datos, puede adjuntarlo a una *VSI*. Adicionalmente, puede crear un nuevo volumen a partir de un *Snapshot* (lo que se denomina restaurar un volumen). Los *Snapshots* son persistentes y tienen un ciclo de vida independiente del volumen original.

La presente guía muestra los pasos que se deben realizar para generar un *Snapshot* que permita crear una copia del volumen de arranque de *Block Storage* de una *VSI* en *VPC*.

<br />

## Índice  📰
1. [Pre-Requisitos](#Pre-Requisitos-pencil)
2. [Crear Snapshot](#Crear-Snapshot-cloud-cd)
3. [Referencias](#Referencias-mag)
4. [Autores](#Autores-black_nib)
<br />


## Pre Requisitos :pencil:
* Contar con una cuenta en <a href="https://cloud.ibm.com/">IBM Cloud</a>.
* Contar con un grupo de recursos.
* Contar con una *VPC*.
* Contar con una *VSI* en *VPC*.

<br />

## Crear Snapshot :cloud: :cd:
Para crear un *Snapshot* del volumen de arranque de *Block Storage* de una *VSI* en *VPC*, siga los pasos que se muestran a continuación:

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
