Ejercicios-PHP-de-suseciones-series-
====================================
<!--Primer Ejercicio de 24-->

            <!--Acosta Alvarado Nexar Jesus
                Tercer Nivel "A"-->
     <title>Primer Ejercicio</title>
     <h1 >Primer Ejercicio</h1>

        <?php
         ini_set('display_errors', 'off');
         ini_set('display_startup_errors', 'off');
         error_reporting(0);
         
        function Primer_Ejercicio(){
            
        $valorx= $_POST['ingresox'];
        $valory= $_POST['ingresoy'];
        
        if ($_POST['enviar']) 
          {
            $valores = ["",7, 6, 8, 4, 9, 2, 10, 0, 11, -2, 12, -4, 13, -6, 14, -8, 15, -10, 16, -12, -17, -14];
            if ($valorx==0 or $valory==0 or $valorx<0 or $valory<0 or $valorx>255 or  $valory>255){
                echo ''-1;
              
            }
           else if ($valores[$valorx] and $valores[$valory]){
                $suma= $valores[$valorx]+$valores[$valory];
                echo 'la suma es : '.$suma;    
            }        
          }else {
       ?>
        <form method="post" action="Primer_ejercicio.php">
            <div>Ingresa X :<input type="text" name="ingresox" maxlength="3"></div>
            <div>Ingresa Y :<input type="text" name="ingresoy" maxlength="3"></div>
            <input type="submit" name="enviar" value="Verificar o Sumar">
         </form>
        
        <?php
               }
        
        } return Primer_Ejercicio();
        ?>
        


<!--Segundo Ejercicio de 24-->

            <!--Acosta Alvarado Nexar
                Tercer Nivel "A"-->
            
 <title>Segundo Ejercicio</title>
 <h1 >Segundo Ejercicio</h1>
 
        <?php
       ini_set('display_errors', 'off');
       ini_set('display_startup_errors', 'off');
       error_reporting(0);
       
       function segundo_ejercicio()
       {
           
       $valorx= $_POST['ingresox'];
       $valory= $_POST['ingresoy'];
       
       if ($_POST['enviar']) 
        {
            $valores_en_x = [2, 2, 4, 12, 48];
            $valores_en_y = [3, 3, 6, 18, 72];
            if ($valorx==0 or $valory==0 or $valorx<0 or $valory<0 or $valorx>255 or  $valory>255){
                echo ''-1;
                return FALSE;
               }
                if ($valorx==2) {
                  $mostrar = $valores_en_x[$valory];
                  echo 'El valor es : '.$mostrar;
               }
             else  if ($valorx==3) {
                  $mostrar = $valores_en_y[$valory];
                  echo 'El valor es : '.$mostrar;
                   
               }
        }else
           {
        ?>
        <form method="post" action="Segundo_ejercicio.php">
            <div>Ingresa X :<input type="text" name="ingresox" maxlength="3"></div>
            <div>Ingresa Y :<input type="text" name="ingresoy" maxlength="3"></div>
            <input type="submit" name="enviar" value="Verificar ">
         </form>
 
        <?php 
          }
        
       } return segundo_ejercicio();
        ?>





<!--tercer Ejercicio de 24-->

            <!--Acosta Alvarado nexar
                Tercer Nivel "A"-->
            
 <title>Tercer Ejercicio</title>
 <h1 >Tercer Ejercicio</h1>
        
     <?php
     ini_set('display_errors', 'off');
     ini_set('display_startup_errors', 'off');
     error_reporting(0); 
     
     function Tercer_ejercicio(){
          $valorx= $_POST['ingresox'];
          $valory= $_POST['ingresoy'];
          
     if ($_POST['enviar']) 
     {
        $valores = ["",60, 30, 20, 15, 12];
        
        if ($valorx==0 or $valory==0 or $valorx<0 or $valory<0 or $valorx>255 or $valory>255) {
            echo ''-1;
        }
        else if ($valorx== $valores[1]) {
            $resultado = $valores[$valory];
             echo ''.$resultado;
        }
        
         
     }else
         {
     ?>
        <form method="post" action="Tercer_ejercicio.php">
            <div>Ingresa X :<input type="text" name="ingresox" maxlength="3"></div>
            <div>Ingresa Y :<input type="text" name="ingresoy" maxlength="3"></div>
            <input type="submit" name="enviar" value="Verificar ">
         </form>
 
    <?php
         }
     }     return Tercer_ejercicio();
    ?>




<!--Cuarto Ejercicio de 24-->

            <!--Acosta Alvarado nexar
                Tercer Nivel "A"-->
        
 <title>Tercer Ejercicio</title>
 <h1 >Tercer Ejercicio</h1>
 
        <?php
     ini_set('display_errors', 'off');
     ini_set('display_startup_errors', 'off');
     error_reporting(0); 
     
     function Cuarto_ejercicio(){
         
         $cadena1= $_POST['S1'];
         $cadena2= $_POST['S2'];
         
     if ($_POST['enviar']) {
         $valor = " ";

             echo ''.$cadena1;
        
         


<!--Quinto Ejercicio de 24-->

            <!--Acosta Alvarado nexar
                Tercer Nivel "A"-->
        
 <title>Quinto Ejercicio</title>
 <h1 >Quinto Ejercicio</h1>
        
     <?php
     ini_set('display_errors', 'off');
     ini_set('display_startup_errors', 'off');
     error_reporting(0); 
     
       function Quinto_ejercicio(){
         
         $matriz= $_POST['valor'];
         $valores = [ 0, 1, 2, 3, 4, 5, 6, 7, 8, 9 ];
         
     if ($_POST['enviar']) {
         if ($matriz == $valores[$matriz]) {
             echo 'La Matriz tiene : <br /><br />'. '[   '.$matriz. '   ]';
           
         }
    else {
         echo 'error';
            
     }
        
         
             
        
         
     }else
         {
        ?>
         <form method="post" action="Quinto_ejercicio.php">
            Ingresa enteros para la matriz :<div><input type="text" name="valor" ></div>
            <input type="submit" name="enviar" value="Verificar ">
         </form>
 
     <?php 
     
        }
     }return Quinto_ejercicio();
     
     ?>

  
         

         
     }else
         {
        ?>
        <form method="post" action="Cuarto_ejercicio.php">
            Ingresa Primer Texto :<div><input type="text" name="S1" maxlength="60"></div>
            Ingresa Segundo Texto :<div><input type="text" name="S2" maxlength="60"></div>
            <input type="submit" name="enviar" value="Verificar ">
         </form>
 
     <?php 
     
        }
     }return Cuarto_ejercicio();
     
     ?>

  
   
