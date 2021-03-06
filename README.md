# VPC - Creaci贸n de Snapshot 馃捇馃捑
*Snapshots for VCP* (instant谩neas para *VPC*) son una oferta regional de *IBM Cloud* que se utiliza para crear una copia puntual de un volumen de datos o de arranque. Para crear un *Snapshot*, el volumen original debe estar adjunto a una instancia de servidor virtual (*VSI*) en ejecuci贸n. El primer *Snapshot* es una copia de seguridad completa del volumen, mientras que los *Snapshots* posteriores del mismo volumen, registran solo los cambios desde la 煤ltima instant谩nea creada. Puede utilizar un *Snapshot* de un volumen de arranque para aprovisionar una instancia. Por otro lado, si el *Snapshot* es de un volumen de datos, puede adjuntarlo a una *VSI*. Adicionalmente, puede crear un nuevo volumen a partir de un *Snapshot* (lo que se denomina restaurar un volumen). Los *Snapshots* son persistentes y tienen un ciclo de vida independiente del volumen original.

La presente gu铆a muestra los pasos que se deben realizar para generar un *Snapshot* que permita crear una copia del volumen de arranque de *Block Storage* de una *VSI* en *VPC*.

<br />

## 脥ndice  馃摪
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
Para crear un *Snapshot* del volumen de arranque de *Block Storage* de una *VSI* en *VPC*, siga los pasos que se muestran a continuaci贸n:

1. En el ```Men煤 de navegaci贸n/Navigation menu``` seleccione la opci贸n ```Infraestructura VPC/VPC Infrastructure```.

2. En la secci贸n de ```Computaci贸n/Compute``` de click la pesta帽a ```Instancias de servidor virtual/Virtual server instances```. Posteriormente, seleccione la *VSI* en la cual desea trabajar. Tenga en cuenta la regi贸n en la que est谩 su *VSI*.

3. Dir铆jase a la secci贸n de ```Vol煤menes de almacenamiento/Storage volumes``` y de click en el ```Vol煤men de arranque/Boot volume``` de la *VSI*.

4. Seleccione la pesta帽a ```Instant谩neas/Snapshots``` y de click en el bot贸n ```Crear +/Create +```.

5. En la nueva ventana complete los campos sugeridos de la siguiente manera:
<br />

**Detalles/Details** 
* ```Nombre/Name```: asigne un nombre exclusivo para su *Snapshot*.
* ```Grupo de recursos/Resource group```: seleccione el grupo de recursos en el cual est谩 trabajando.
* ```Regi贸n/Region```: indique la regi贸n en donde est谩 trabajando.
<br />

**Volumen/Volume**
* Seleccione el volumen de almacenamiento sobre el que quiere crear el *Snapshot*.
<br />

6. De click en el bot贸n ```Crear instant谩nea/Creat snapshot``` y espere unos minutos mientra se completa la solicitud para la creaci贸n del *Snapshot*.

7. Refresque la secci贸n de los *Snapshots* con la opci贸n 馃攧 y espere mientra se completa el proceso.

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
