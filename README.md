# praktika2ikbo16-17-Boldyrev-Grigoriy

Класс автор

import java.lang.*;
public class Author {
    private String name ; private String email ; private char gender ;
    public Author(String name, String email,  char gen) {
        this.name = name;
        this.email = email;
        gender = gen;

        if (gender == 'M') {
            gender = 'M';

        } else if (gender == 'U') {
            gender = 'U';

        } else if (gender == 'F')

        {
            gender = 'F';
        }
    }
    public String toString()
    {
        return ("Author: " + getName() + " Gender " + getGender()+" "+ "at " + getEmail());
    }

    public void setEmail( String em)
    {
        email=em;

    }

    public String getName()
    {
        return name;
    }

    public String getEmail()
    {
        return email;
    }
    public char getGender()
    {
        return gender;

}
}

Класс Тестер

public class TestAuthor {
    public static void main(String[] args) {
        Author at = new Author("J.K. Rowling", "JRowling@gmail.com", 'F');
        System.out.println(at.toString());

    }
}
