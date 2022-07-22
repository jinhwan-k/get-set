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




연습문제

1) Tutor 클래스를 만들고, 이름(name)과, 경력(bio) 멤버 변수를 추가하세요.
2) 그리고 각 변수를 private 으로 선언하고, Getter와 Setter 를 만들어보세요.
3) 마지막으로, 기본 생성자와, name/bio 입력받는 생성자 두 개를 만들어보세요.

public class Tutor {                            
    // 멤버 변수
    private String name;
    private String bio;
    
    // 기본생성자
    public Tutor() {
        
    }
    
    // 생성자
    public Tutor(String name, String bio) {
        this.name = name;
        this.bio = bio;
    }
    
    // Getter
    public String getName() {
        return this.name;
    }
    public String getBio() {
        return this.bio;
    }
    
    // Setter    
    public void setName(String name) {
        this.name = name;
    }
    public void setBio(String bio) {
        this.bio = bio;
    }
    
}

자주봐봐야겠다.
