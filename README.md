# AccountBook
JavaFX, MySQL, JDBC를 사용해 구현한 가계부 애플리케이션


<h3> MVC (MODEL VIEW CONTROL) 패턴을 사용해 구현 </h3>
<ul>
<li>MODEL  : Calendar, CalendarService, ReloadEvent, 등에 클래스이며 프로그램에 전체적인 흐름을 조절하는데 도와주는 도구들이다.</li>
<li>CONTROL : CalenderController, CalenderModalController, SideController 등에 Controller 클래스이며 VIEW 랑 연동되어 조절해주는 클래스들이다.</li>
<li>VIEW : FXML, CSS 파일 모드 VIEW이며 실제 프로그램에 디자인을 구현하는데 사용된다.</li>
</ul>




<h3> 클래스 설명 </h3>
<ul>
<li>Calendar : 수입/지출 기록 내역을 저장하는 객체</li>
<li>CalendarService : MySQL 데이터베이스 관리하는 객체</li>
<li>CalendarController : calender-view.fxml 캘런더 창 기능 구현</li>
<li>CalendarModalController : calender-modal.fxml 캘런더 기록하기 창 기능 구현</li>
<li>SideController : side-view.fxml 캘런더 창 기능 구현</li>
..... 등 모든 Controller는 자기 이름과 동일한 fxml과 연동되어 기능 구현하는 역할함 Modal가 붙여있으면 팦업 창을 담당함

</ul>

<h3> FXML,CSS 설명 </h3>
<ul>
<li>FXML : calender-view는 캘런터 창에 있는 모든 element 또는 요소를 구현하며 side-view는 옆창을 구현한다. 그냥 HTML 파일이다고 생가하면 된다</li>
<li>CSS : FXML 파일에 있는 element 요소를 디자인 하는데 사용된다. calendar.css는 캘런더 창 디자인, side.css 는 옆창 디자인 등,</li>
</ul>
