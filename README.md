# interactive

$dayofweek = (Get-date).DayOfWeek
$currenthour = (get-date).Hour

if ($env:USERNAME -contains "yassi")
{
    if (($dayofweek -ne "Monday" -or $dayofweek -ne "Thursday" -or $dayofweek -ne "Friday") -and (($currenthour -lt 16 -or $currenthour -gt 19))){
  #echo ok
  logoff  
}

}
