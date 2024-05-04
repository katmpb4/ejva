<?php
//Szukalski Marek
//www.algorytm.org
//sortowanie babelkowe
 
$tabela=array('12','123','1','5','756','234','43','24');
//pamietajmy, że indeks w tabeli rozpoczyna sie od 0
//a konczy na n-1
 
$n=8; //ilosc elementow w tabeli
 
for($i=$n;$i>=0;$i--){//petla glowna      
 
for($j=0;$j<$i-1;$j++){//petla wewnetrzna
 
if($tabela[$j]>$tabela[$j+1]){ //warunek
$tmp=$tabela[$j];   //zamiana
$tabela[$j]=$tabela[$j+1];
$tabela[$j+1]=$tmp;
}
}
}
 
for($i=0;$i<$n;$i++) echo($tabela[$i].'  '); //wypisanie posortowanych wartosci tabeli
 
?>
