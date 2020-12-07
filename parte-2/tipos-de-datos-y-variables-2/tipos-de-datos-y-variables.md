# Requerimientos para Python

![](../../.gitbook/assets/portada_python_bedu_open_vid02.png)

### 👩💻 **Requerimientos**

Puedes desarrollar en Python en cualquier Sistema Operativo, ya sea **Mac**, **Linux** o **Windows**. Recomendamos el uso de sistemas operativos basados en **UNIX** \(**Mac** o **Linux**\).

Durante el desarrollo de este curso, será necesario tengas instalados en tu computadora un editor de texto \(Recomendamos **Visual Studio Code**\) y **Python**.

En los sistemas operativos **Mac** y **Linux** ya se encuentra instalado en el sistema, pero para descargar la versión más actual incluyendo **Windows** se puede realizar por medio del siguiente recurso

{% embed url="https://www.python.org/downloads/" %}

### **Editor de texto recomendado**

> ![](../../.gitbook/assets/1200px-visual_studio_code_1.18_icon.svg.png) **Visual Studio Code** 
>
> **Selecciona la descarga de Visual Studio Code dependiendo de tu sistema operativo:**
>
> \*\*\*\*![](../../.gitbook/assets/icons8-windows-10-480.png) **Windows:**
>
> * **Windows** de ****[**64 bit**](https://code.visualstudio.com/docs/?dv=win64user)
> * **Windows** de ****[**32 bit**](https://code.visualstudio.com/docs/?dv=win32user)
>
> \*\*\*\*![](../../.gitbook/assets/1200px-apple_logo_black.svg.png) **Mac:**
>
> * Descarga de Visual Studio Code ****para ****[**Mac**](https://code.visualstudio.com/docs/?dv=osx)
>
> \*\*\*\*![](../../.gitbook/assets/icons8-linux-96.png) **Linux:**
>
> * **Linux:** [**\(Debian, Ubuntu\)**](https://code.visualstudio.com/docs/?dv=linux64_deb)
> * **Linux:** [**\(Red Hat, Fedora, SUSE\)**](https://code.visualstudio.com/docs/?dv=linux64_rpm)
>
> **Es importante que tu computadora cumpla con los siguientes requerimientos para instalar Visual Studio Code:**
>
> * **Sistema Operativo Mínimo:** 
>
>   * Windows 7
>   * OS X Yosemite o superior
>   * Ubuntu 14.04 o Debian 7
>   * Red Hat 7, CentOS7, Fedora 23
>
>   \*\*\*\*
>
> * **Velocidad mínima de Procesador:** 1.6Ghz
> * **Memoria RAM mínima:** 1Gb

### **Manual de Instalación de Python 3 en Mac**

**OS X** viene con un gran número de utilidades de desarrollo y es posible trabajar con **Python** sin instalar software adicional, pero generalmente cuenta con la **versión 2.7** que actualmente se encuentra sin soporte.

Para instalar la versión más actual en OS X será necesario instalar xCode desde la App Store

{% embed url="https://apps.apple.com/mx/app/xcode/id497799835?mt=12" %}

Una vez descargado será necesario abrir la terminal y ejecutar el siguiente comando: ****`xcode-select --install`

![](https://lh3.googleusercontent.com/8xVs5wy6b3ED1u7vBy7ea84lqGVaTKOZ9rhO7FjydB60eUK8bet2XcgwVsN0LaZWh3UbStSAEknaD5YbY8FZlYokMQX519zE-5n6k7I5HF2g0OCwkrAphvCs9cMm4aKaE9PK4050)

Una vez termine la ejecución del comando será necesario instalar **Homebrew** por medio del siguiente comando: `$ ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"`

![](https://lh6.googleusercontent.com/Rep61c0FMEDJG5-OFgEHbXEP_ty4g1HdFrZfXryVt0TnxYbxjQ2g2mmRrCl2fzphlT2qFirQF6PJinyWp7HM_hSQ2U76WV2KKUnRCrOfUcGoJ9jBJRQe9h3b9aNcYWZuL-Tpl0zY)

![](https://lh3.googleusercontent.com/zGw2BAzXijuhkh3IlTYVtZbFN0GG8F39gciz8xmits6gGEqIoxiJkt9pmtRwoL0K28ZsqkqL60CuZ5bmu7aWeOla8oKAt-Ov7p8pySTrxx01TAEokRFE_umHIxg4Gl_1s-OpOCDN)

![](https://lh6.googleusercontent.com/HtNkRYW0Hc-XbcbdUTQLWlXctMMUYr8bjLmvsk96aPMxqiCbmni95OyY0bBFOEnbpDmJOudtMxYC1BqPi1Poph1jIEYsMP1zbXqdTsDcsLuaKQapxo_2IoO0Z79ST_VXEQrZE31h)

Una vez termine la descarga de **brew** en nuestro sistema podemos instalar Python 3 con el siguiente comando: `brew install python3`

![](https://lh4.googleusercontent.com/lKGmAXnJJJbiutn_y_MpjHBi5px-7ljdMNB7rz7VqwD7m3Y4WKR9gDo_HNTtncaTxl9mDYSGGBUul8QbVC2DKd4ktw238_QYZDzVpfcWX-8Wi_niJhPPcaHxMSs4HuHpOmK0aqyw)

Una vez termine de ejecutarse el comando, tendremos instalado **python 3** en nuestro sistema, para verificar la instalación fue exitosa ejecutamos el siguiente comando: `python3`

![](https://lh4.googleusercontent.com/4M1gT7BYynHONo07eSSDT25yygdL9MSTd3zaDTDkdCYMZhErDDCRjWijCe_A5A7rPSayUbZCZG32jvgVSq4gAkTjbfGMaWJ99Kyv1F6H5_k9K296xtaKbIP1Y285Tp3OjfRC_IPU)

### **Manual de Instalación de Python 3 en Windows**

Primero debemos **descargar** la última versión de Python desde el sitio oficial, en el siguiente link podrás encontrar las opciones de descarga:

{% embed url="https://www.python.org/downloads/" %}

Una vez descargado el instalador lo ejecutamos y veremos la siguiente pantalla, donde **activaremos** **la** **casilla** **Add Python Path** y realizaremos click en la leyenda **Install Now**

![](https://lh6.googleusercontent.com/9HWMUtNxtJbp2AaIxHPCqYnx2OgGHBKFfqSMvEGrkRYVlUci42f85QWu0w6ay0tYL-XaUKkn1kpxyN3PAhnqY_vNd4v2YRgzn83Ny-CggGyX_mXsLPO2_FJ5iFaZMI2Hi2v0KyU2)

![](https://lh4.googleusercontent.com/urTzxXnTcj9OASzgZ-odfXucxYHJWEZ86ujAlSJplmuExfCggJn6U2zkat0Yv9saaAiq1x4LILZXPle2_0La17QkwtJzsVyGRDvvtulh0LSKwZbn6Kfu2TAl8YzB6h1Jd_mnBpA-)

Una vez termine la instalación veremos la siguiente pantalla

![](https://lh3.googleusercontent.com/F6m0GwoBn-QxRdJx6NnGJGSF524C0kKEnkXuplkSXZBolBXmimycpmfH3FHVmKqf4_SHfeX9Niev1eBWvGiGh6i2UsA8JEN44_MIC1pyLndzTaAYRs4i1tUA3FvgoHGKjivwF8B0)

En nuestro buscador del sistema operativo **buscaremos** **Python** y encontraremos la **app** a **ejecutar**, realizaremos click y tendremos en pantalla la siguiente terminal 

![](https://lh5.googleusercontent.com/4M7s0OTsBTNqSqowJfCR_t-toATTEKhrk2mGPg--MBbOer0nDaiu_x6zStb7tuyFWJNRdJwCPQW7cbJJdmORNhlABPkKthXSw7hVTZepkLqfeMGX-P0EqASJT8UB_GQxNSsWNd0D)

Una vez instalado todos los requerimientos del curso es **momento de iniciar con el primer tema.**

