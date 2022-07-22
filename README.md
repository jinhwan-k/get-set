# get-set

정보를 가져오는 메소드를 Getter,
정보를 바꾸는 메소드를 Setter 라고 부른다.

얘들이 존재하는 이유는 public으로 설정하면 중요한 정보가 가볍고 쉽게 바뀔수있기에
미리 방지하기위해 get,set으로 설정한다. 한마디로 이중,삼중 확인해서 바꿔라.인것같다.

// Getter                             // Setter
public String getTitle() {            public void setTitle(String title) {
    return this.title;                    this.title = title;                                       
}                                      }
// Getter                             // Setter
public String getTutor() {             public void setTutor(String tutor) {
    return this.tutor;                     this.tutor = tutor;
}                                      }
// Getter                             // Setter
public int getDays() {                public void setDays(int days) {
    return this.days;                      this.days = days;
}                                     }


해서 prac폴더를 고치면

Course course = new Course();

System.out.println(course.getTitle());
System.out.println(course.getTutor());
System.out.println(course.getDays());

course.setTitle("웹개발의 봄 스프링");
course.setTutor("남병관");
course.setDays(35);

System.out.println(course.getTitle());
System.out.println(course.getTutor());
System.out.println(course.getDays());


