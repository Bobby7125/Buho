Inicio () {
        clear
printf "$P Hyliana:$C ¿Cual Metodo Usaras?"
echo                                                                       printf "\n"                                                                printf "$C=================================\e[0m\n"
printf "$C[\e[0m01$C]$V Wen Site Fake\e[0m\n"
printf "$C[\e[0m02$C]$V Mac Del Router\e[0m\n"
printf "$C[\e[0m03$C]$V Ubicacion Aproximada Con IP\e[0m\n"
printf "$C=================================\e[0m\n"
echo
read -p $'\e[1;96m[\e[0m\e[1;77m*\e[0m\e[1;96m]\e[1;95m Hyliana:\e[1;92m Escoja Una Opción >> \e[0m' opc
                                                                   if [[ $o
pc == 1 || $opc == 01 ]]; then
                                                                    Web
                                                                   elif [[
$opc == 2 || $opc == 02 ]]; then
                                                                   MAC     
     elif [[ $opc == 3 || $opc == 03 ]]; then

             EIP
        else

printf "$A[$R!$A] ¡Upss! ¡Opcion No Valida!"

        Inicio
                                                                  fi

}

MAC () {                                                                  clear
banner
echo
echo
  rm -rf Datos/datos.json
printf "$C[*]$P ¡Hyliana:$V El Buho Recorre Todo El Mundo!\n"
echo                                                                       printf "$V+===========================================+\n"                 printf "$B Al Buho Terminar De Recorrer Todo El Mundo\n"
printf "$B Te Lanza La Ubicacion Precisa Del Router De\n"                  printf "$B La Victima.$A Debes  De Colocar La Mac Del\n"
printf "$A Router Como El Ejemplp  Y Todas Las Letras\n"
printf "$A En Mayuscula. ¡Gracias Por Elegirme...!\n"                      printf "$V+===========================================+\n"
printf "$A[$R!$A]$P Hyliana:$R Ejemplo$V Coloque Mac Victima >>\e[0m 00:00
:00:00:00\n"
          echo                                                                       echo
          echo

read -p $'\e[1;96m[\e[0m\e[1;77m*\e[0m\e[1;96m]\e[1;95m Hyliana:\e[1;92m C
oloque Mac Victima >> \e[0m' mac

   if [[ $mac >  00:00:00:00:00 ]]; then

     curl "https://api.mylnikov.org/geolocation/wifi?v=1.2&bssid=$mac" > /d
ev/null 2>&1 >  Datos/datos.json                                              else
           echo
           printf "$A [$R!$A]$R Mac Invalida! "
           echo
           sleep 3
     fi                                                                    

  Time=$(cat "Datos/datos.json" | jq '.data' | jq ".time")

  Range=$(cat "Datos/datos.json" | jq '.data' | jq ".range")               
  Latitud=$(cat "Datos/datos.json" | jq '.data' | jq  ".lat")

  Longitud=$(cat "Datos/datos.json" | jq '.data' | jq ".lon")

  Maps=https://www.google.com/maps/place/$Latitud+$Longitud

echo                                                                       if [[ $Latitud  == null ]]; then

       printf "$R [-]$A Time: No Encontrado...\e[0m\n"


       printf "$R [-]$A Range: No Encotrado...\e[0m\n"
                                                                                                                                                             printf "$R [-]$A Latitud: No Encotrado...\e[0m\n"
                                                                           
       printf "$R [-]$A Longitud: No Encotrado...\e[0m\n"
                                                                           
       printf "$R [-]$A Google Maps: No Disponible...\e[0m\n"
  echo
   else                                                                       printf "$C[$B*$C] $P Hyliana:\e[0m Obteniendo Ubicacion De La Victima...
."
      echo

       sleep 5
echo
printf "$V [+]$C Time:\e[0m $Time \e[0m\n"
echo
sleep 0.5
printf "$V [+]$C Range:\e[0m $Range \e[0m\n"                               echo
sleep 0.5
printf "$V [+]$C Latitud:\e[0m $Latitud \e[0m\n"
echo
sleep 0.5
printf "$V [+]$C Longitud:\e[0m $Longitud \e[0m\n"                         echo
sleep 0.9
printf "$V [+]$C Google Maps:\e[0m $Maps \e[0m\n"
sleep 5
fi                                                                        



}
