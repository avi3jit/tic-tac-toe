# tic-tac-toe
website similar to urban-clap as my furst project
<!DOCTYPE html>
<head>
  <title>
    TIC - TAC-TOE
  </title>
  <style>
  th,td{
    padding:5%;
    border:5px solid red;
  }
  </style>
</head>
<body>
  <div id="h11" >
    <br>
    this is the turn of O
  </div>
  <table style="background-color:rgb(0,0,200);color:white;width:30%;margin-left:10%">
    <tr>
      <td id="a1" onclick=func1()>

</td>
      <td id="a2" onclick=func2()>

</td>
      <td id="a3" onclick=func3()>

</td>
    </tr>
    <tr>
      <td id="b1" onclick=func4()>

      </td>
      <td id="b2" onclick=func5()>

      </td>
      <td id="b3" onclick=func6()>

      </td>
    </tr>
    <tr>
      <td id="c1" onclick=func7()>

      </td>
      <td id="c2" onclick=func8()>

      </td>
      <td id="c3" onclick="func9()">

      </td>
    </tr>
  </table>
  <div id="h22" onclick="func10()">
    <h2> PLAY AGAIN</h2>
  </div>
  <p id="result">
  </p>
  <script>
  var turn=1;var arr=["0","0","0","0","0","0","0","0","0"];var q=0;
  function func10()
  {
    location.reload();
  }


   function func1()
  { turn=turn+1;

    if(turn%2==1)
    {
        document.getElementById("h11").innerHTML = "this is turn of O";

    }
    else {


          document.getElementById("h11").innerHTML = "this is the turn of X";

    }
    if(turn%2==1)
    {document.getElementById("a1").innerHTML = "X";arr[0]=1;}
else {
  document.getElementById("a1").innerHTML = "O";arr[0]=2;
}
if(turn>=5)
{  if((arr[0]==1&&arr[1]==1&&arr[2]==1)||(arr[3]==1&&arr[4]==1&&arr[5]==1)||(arr[6]==1&&arr[7]==1&&arr[8]==1)||(arr[0]==1&&arr[3]==1&&arr[6]==1)||
(arr[1]==1&&arr[4]==1&&arr[7]==1)||(arr[2]==1&&arr[5]==1&&arr[8]==1)||(arr[6]==1&&arr[4]==1&&arr[2]==1)||(arr[0]==1&&arr[4]==1&&arr[8]==1))
{
    document.getElementById("h11").innerHTML = "X HAS WON!!HURRAY";q=1;
}
if((arr[0]==2&&arr[1]==2&&arr[2]==2)||(arr[3]==2&&arr[4]==2&&arr[5]==2)||(arr[6]==2&&arr[7]==2&&arr[8]==2)||(arr[0]==2&&arr[3]==2&&arr[6]==2)||
(arr[1]==2&&arr[4]==2&&arr[7]==2)||(arr[2]==2&&arr[5]==2&&arr[8]==2)||(arr[6]==2&&arr[4]==2&&arr[2]==2)||(arr[0]==2&&arr[4]==2&&arr[8]==2))
{
    document.getElementById("h11").innerHTML = "O HAS WON!!HURRAY";q=1;
}
}
if(turn==10&&q==0)
  document.getElementById("h11").innerHTML = "DRAWN";}
  function func2()
    { turn=turn+1;

      if(turn%2==1)
      {
          document.getElementById("h11").innerHTML = "this is turn of O";

      }
      else {


            document.getElementById("h11").innerHTML = "this is the turn of X";

      }
      if(turn%2==1)
      {document.getElementById("a2").innerHTML = "X";arr[1]=1;
    }
    else {
      document.getElementById("a2").innerHTML = "O";arr[1]=2;
    }
    if(turn>=5)
    {  if((arr[0]==1&&arr[1]==1&&arr[2]==1)||(arr[3]==1&&arr[4]==1&&arr[5]==1)||(arr[6]==1&&arr[7]==1&&arr[8]==1)||(arr[0]==1&&arr[3]==1&&arr[6]==1)||
    (arr[1]==1&&arr[4]==1&&arr[7]==1)||(arr[2]==1&&arr[5]==1&&arr[8]==1)||(arr[6]==1&&arr[4]==1&&arr[2]==1)||(arr[0]==1&&arr[4]==1&&arr[8]==1))
    {
        document.getElementById("h11").innerHTML = "X HAS WON!!HURRAY";q=1;
    }
    if((arr[0]==2&&arr[1]==2&&arr[2]==2)||(arr[3]==2&&arr[4]==2&&arr[5]==2)||(arr[6]==2&&arr[7]==2&&arr[8]==2)||(arr[0]==2&&arr[3]==2&&arr[6]==2)||
    (arr[1]==2&&arr[4]==2&&arr[7]==2)||(arr[2]==2&&arr[5]==2&&arr[8]==2)||(arr[6]==2&&arr[4]==2&&arr[2]==2)||(arr[0]==2&&arr[4]==2&&arr[8]==2))
    {
        document.getElementById("h11").innerHTML = "O HAS WON!!HURRAY";q=1;
    }
    }
    if(turn==10&&q==0)
      document.getElementById("h11").innerHTML = "DRAWN";}
    function func3()
      { turn=turn+1;

        if(turn%2==1)
        {
            document.getElementById("h11").innerHTML = "this is turn of O";

        }
        else {


              document.getElementById("h11").innerHTML = "this is the turn of X";

        }
        if(turn%2==1)
        {document.getElementById("a3").innerHTML = "X";arr[2]=1;
      }
      else {
        document.getElementById("a3").innerHTML = "O";arr[2]=2;
      }
      if(turn>=5)
      {  if((arr[0]==1&&arr[1]==1&&arr[2]==1)||(arr[3]==1&&arr[4]==1&&arr[5]==1)||(arr[6]==1&&arr[7]==1&&arr[8]==1)||(arr[0]==1&&arr[3]==1&&arr[6]==1)||
      (arr[1]==1&&arr[4]==1&&arr[7]==1)||(arr[2]==1&&arr[5]==1&&arr[8]==1)||(arr[6]==1&&arr[4]==1&&arr[2]==1)||(arr[0]==1&&arr[4]==1&&arr[8]==1))
      {
          document.getElementById("h11").innerHTML = "X HAS WON!!HURRAY";q=1;
      }
      if((arr[0]==2&&arr[1]==2&&arr[2]==2)||(arr[3]==2&&arr[4]==2&&arr[5]==2)||(arr[6]==2&&arr[7]==2&&arr[8]==2)||(arr[0]==2&&arr[3]==2&&arr[6]==2)||
      (arr[1]==2&&arr[4]==2&&arr[7]==2)||(arr[2]==2&&arr[5]==2&&arr[8]==2)||(arr[6]==2&&arr[4]==2&&arr[2]==2)||(arr[0]==2&&arr[4]==2&&arr[8]==2))
      {
          document.getElementById("h11").innerHTML = "O HAS WON!!HURRAY";q=1;
      }
      }
      if(turn==10&&q==0)
        document.getElementById("h11").innerHTML = "DRAWN";}
      function func4()
        {turn=turn+1;

          if(turn%2==1)
          {
              document.getElementById("h11").innerHTML = "this is turn of O";

          }
          else {


                document.getElementById("h11").innerHTML = "this is the turn of X";

          }
           if(turn%2==1)
          {document.getElementById("b1").innerHTML = "X";arr[3]=1;
        }
        else {
          document.getElementById("b1").innerHTML = "O";arr[3]=2;
        }
        if(turn>=5)
        {  if((arr[0]==1&&arr[1]==1&&arr[2]==1)||(arr[3]==1&&arr[4]==1&&arr[5]==1)||(arr[6]==1&&arr[7]==1&&arr[8]==1)||(arr[0]==1&&arr[3]==1&&arr[6]==1)||
        (arr[1]==1&&arr[4]==1&&arr[7]==1)||(arr[2]==1&&arr[5]==1&&arr[8]==1)||(arr[6]==1&&arr[4]==1&&arr[2]==1)||(arr[0]==1&&arr[4]==1&&arr[8]==1))
        {
            document.getElementById("h11").innerHTML = "X HAS WON!!HURRAY";q=1;
        }
        if((arr[0]==2&&arr[1]==2&&arr[2]==2)||(arr[3]==2&&arr[4]==2&&arr[5]==2)||(arr[6]==2&&arr[7]==2&&arr[8]==2)||(arr[0]==2&&arr[3]==2&&arr[6]==2)||
        (arr[1]==2&&arr[4]==2&&arr[7]==2)||(arr[2]==2&&arr[5]==2&&arr[8]==2)||(arr[6]==2&&arr[4]==2&&arr[2]==2)||(arr[0]==2&&arr[4]==2&&arr[8]==2))
        {
            document.getElementById("h11").innerHTML = "O HAS WON!!HURRAY";q=1;
        }
        }
        if(turn==10&&q==0)
          document.getElementById("h11").innerHTML = "DRAWN";}
        function func5()
          {turn=turn+1;

            if(turn%2==1)
            {
                document.getElementById("h11").innerHTML = "this is turn of O";

            }
            else {


                  document.getElementById("h11").innerHTML = "this is the turn of X";

            }
             if(turn%2==1)
            {document.getElementById("b2").innerHTML = "X";arr[4]=1;
          }
          else {
            document.getElementById("b2").innerHTML = "O";arr[4]=2;
          }
          if(turn>=5)
          {  if((arr[0]==1&&arr[1]==1&&arr[2]==1)||(arr[3]==1&&arr[4]==1&&arr[5]==1)||(arr[6]==1&&arr[7]==1&&arr[8]==1)||(arr[0]==1&&arr[3]==1&&arr[6]==1)||
          (arr[1]==1&&arr[4]==1&&arr[7]==1)||(arr[2]==1&&arr[5]==1&&arr[8]==1)||(arr[6]==1&&arr[4]==1&&arr[2]==1)||(arr[0]==1&&arr[4]==1&&arr[8]==1))
          {
              document.getElementById("h11").innerHTML = "X HAS WON!!HURRAY";q=1;
          }
          if((arr[0]==2&&arr[1]==2&&arr[2]==2)||(arr[3]==2&&arr[4]==2&&arr[5]==2)||(arr[6]==2&&arr[7]==2&&arr[8]==2)||(arr[0]==2&&arr[3]==2&&arr[6]==2)||
          (arr[1]==2&&arr[4]==2&&arr[7]==2)||(arr[2]==2&&arr[5]==2&&arr[8]==2)||(arr[6]==2&&arr[4]==2&&arr[2]==2)||(arr[0]==2&&arr[4]==2&&arr[8]==2))
          {
              document.getElementById("h11").innerHTML = "O HAS WON!!HURRAY";q=1;
          }
          }
          if(turn==10&&q==0)
            document.getElementById("h11").innerHTML = "DRAWN";}
          function func6()
            { turn=turn+1;

              if(turn%2==1)
              {
                  document.getElementById("h11").innerHTML = "this is turn of O";

              }
              else {


                    document.getElementById("h11").innerHTML = "this is the turn of X";

              }
               if(turn%2==1)
              {document.getElementById("b3").innerHTML = "X";arr[5]=1;
            }
            else {
              document.getElementById("b3").innerHTML = "O";arr[5]=2;
            }
            if(turn>=5)
            {  if((arr[0]==1&&arr[1]==1&&arr[2]==1)||(arr[3]==1&&arr[4]==1&&arr[5]==1)||(arr[6]==1&&arr[7]==1&&arr[8]==1)||(arr[0]==1&&arr[3]==1&&arr[6]==1)||
            (arr[1]==1&&arr[4]==1&&arr[7]==1)||(arr[2]==1&&arr[5]==1&&arr[8]==1)||(arr[6]==1&&arr[4]==1&&arr[2]==1)||(arr[0]==1&&arr[4]==1&&arr[8]==1))
            {
                document.getElementById("h11").innerHTML = "X HAS WON!!HURRAY";q=1;
            }
            if((arr[0]==2&&arr[1]==2&&arr[2]==2)||(arr[3]==2&&arr[4]==2&&arr[5]==2)||(arr[6]==2&&arr[7]==2&&arr[8]==2)||(arr[0]==2&&arr[3]==2&&arr[6]==2)||
            (arr[1]==2&&arr[4]==2&&arr[7]==2)||(arr[2]==2&&arr[5]==2&&arr[8]==2)||(arr[6]==2&&arr[4]==2&&arr[2]==2)||(arr[0]==2&&arr[4]==2&&arr[8]==2))
            {
                document.getElementById("h11").innerHTML = "O HAS WON!!HURRAY";q=1;
            }
            }
            if(turn==10&&q==0)
              document.getElementById("h11").innerHTML = "DRAWN";}
            function func7()
              {turn=turn+1;

                if(turn%2==1)
                {
                    document.getElementById("h11").innerHTML = "this is turn of O";

                }
                else {


                      document.getElementById("h11").innerHTML = "this is the turn of X";

                }
                 if(turn%2==1)
                {document.getElementById("c1").innerHTML = "X";arr[6]=1;
              }
              else {
                document.getElementById("c1").innerHTML = "O";arr[6]=2;
              }if(turn>=5)
              {  if((arr[0]==1&&arr[1]==1&&arr[2]==1)||(arr[3]==1&&arr[4]==1&&arr[5]==1)||(arr[6]==1&&arr[7]==1&&arr[8]==1)||(arr[0]==1&&arr[3]==1&&arr[6]==1)||
              (arr[1]==1&&arr[4]==1&&arr[7]==1)||(arr[2]==1&&arr[5]==1&&arr[8]==1)||(arr[6]==1&&arr[4]==1&&arr[2]==1)||(arr[0]==1&&arr[4]==1&&arr[8]==1))
              {
                  document.getElementById("h11").innerHTML = "X HAS WON!!HURRAY";q=1;
              }
              if((arr[0]==2&&arr[1]==2&&arr[2]==2)||(arr[3]==2&&arr[4]==2&&arr[5]==2)||(arr[6]==2&&arr[7]==2&&arr[8]==2)||(arr[0]==2&&arr[3]==2&&arr[6]==2)||
              (arr[1]==2&&arr[4]==2&&arr[7]==2)||(arr[2]==2&&arr[5]==2&&arr[8]==2)||(arr[6]==2&&arr[4]==2&&arr[2]==2)||(arr[0]==2&&arr[4]==2&&arr[8]==2))
              {
                  document.getElementById("h11").innerHTML = "O HAS WON!!HURRAY";q=1;
              }
              }
              if(turn==10&&q==0)
                document.getElementById("h11").innerHTML = "DRAWN";}
              function func8()
                {turn=turn+1;

                  if(turn%2==1)
                  {
                      document.getElementById("h11").innerHTML = "this is turn of O";

                  }
                  else {


                        document.getElementById("h11").innerHTML = "this is the turn of X";

                  }
                   if(turn%2==1)
                  {document.getElementById("c2").innerHTML = "X";arr[7]=1;
                }
                else {
                  document.getElementById("c2").innerHTML = "O";arr[7]=2;
                }
                if(turn>=5)
                {  if((arr[0]==1&&arr[1]==1&&arr[2]==1)||(arr[3]==1&&arr[4]==1&&arr[5]==1)||(arr[6]==1&&arr[7]==1&&arr[8]==1)||(arr[0]==1&&arr[3]==1&&arr[6]==1)||
                (arr[1]==1&&arr[4]==1&&arr[7]==1)||(arr[2]==1&&arr[5]==1&&arr[8]==1)||(arr[6]==1&&arr[4]==1&&arr[2]==1)||(arr[0]==1&&arr[4]==1&&arr[8]==1))
                {
                    document.getElementById("h11").innerHTML = "X HAS WON!!HURRAY";q=1;
                }
                if((arr[0]==2&&arr[1]==2&&arr[2]==2)||(arr[3]==2&&arr[4]==2&&arr[5]==2)||(arr[6]==2&&arr[7]==2&&arr[8]==2)||(arr[0]==2&&arr[3]==2&&arr[6]==2)||
                (arr[1]==2&&arr[4]==2&&arr[7]==2)||(arr[2]==2&&arr[5]==2&&arr[8]==2)||(arr[6]==2&&arr[4]==2&&arr[2]==2)||(arr[0]==2&&arr[4]==2&&arr[8]==2))
                {
                    document.getElementById("h11").innerHTML = "O HAS WON!!HURRAY";q=1;
                }
              }if(turn==10&&q==0)
                  document.getElementById("h11").innerHTML = "DRAWN";}
                function func9()
                  {turn=turn+1;

                    if(turn%2==1)
                    {
                        document.getElementById("h11").innerHTML = "this is turn of O";

                    }
                    else {


                          document.getElementById("h11").innerHTML = "this is the turn of X";

                    }
                     if(turn%2==1)
                    {document.getElementById("c3").innerHTML = "X";arr[8]=1;
                  }
                  else {
                    document.getElementById("c3").innerHTML = "O";arr[8]=2;
                  }
                  if(turn>=5)
                  {  if((arr[0]==1&&arr[1]==1&&arr[2]==1)||(arr[3]==1&&arr[4]==1&&arr[5]==1)||(arr[6]==1&&arr[7]==1&&arr[8]==1)||(arr[0]==1&&arr[3]==1&&arr[6]==1)||
                  (arr[1]==1&&arr[4]==1&&arr[7]==1)||(arr[2]==1&&arr[5]==1&&arr[8]==1)||(arr[6]==1&&arr[4]==1&&arr[2]==1)||(arr[0]==1&&arr[4]==1&&arr[8]==1))
                  {
                      document.getElementById("h11").innerHTML = "X HAS WON!!HURRAY";q=1;
                  }
                  if((arr[0]==2&&arr[1]==2&&arr[2]==2)||(arr[3]==2&&arr[4]==2&&arr[5]==2)||(arr[6]==2&&arr[7]==2&&arr[8]==2)||(arr[0]==2&&arr[3]==2&&arr[6]==2)||
                  (arr[1]==2&&arr[4]==2&&arr[7]==2)||(arr[2]==2&&arr[5]==2&&arr[8]==2)||(arr[6]==2&&arr[4]==2&&arr[2]==2)||(arr[0]==2&&arr[4]==2&&arr[8]==2))
                  {
                      document.getElementById("h11").innerHTML = "O HAS WON!!HURRAY";q=1;
                  }
                  }
                  if(turn==10&&q==0)
                    document.getElementById("h11").innerHTML = "DRAWN";}








</script>
</body>
</html>
