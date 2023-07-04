# Visualization_Idea_Note

1. Invoice 만료일이 지난 후에 clear된 경우 채권 회수에 위험이 뒤따를 수 있음.</br> 따라서 만료일 후 clear된 횟수, 금액이 많은 경우에는 유의할 필요가 있음.</br>
develop) </br>
만료일 이후 clear된 횟수와 금액의 추이를 확인할 필요가 있음.</br> 빈도와 금액이 높아지는 추세를 보이는 경우 더 경계해야함.</br>

2. 일별로 그룹 / 매일 만료일이 지났으나 clear가 안 된 경우.

오늘 날짜 / due date / clear date

오늘 날짜 > due date AND (clear date == Null OR clear date > 오늘 날짜)
but
clear date는 늦게라도 채워짐.
clear date > 오늘 날짜

3. 매출채권 Default</br>
매출채권을 일정 기간동안 회수하지 못하면 Default로 정의</br>
기간에 대한 정의가 필요할 것</br>
1번과 다소 겹칠 수 있음으로 어떤 항목을 유지할지 정해야함