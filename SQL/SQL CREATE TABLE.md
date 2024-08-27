[[SQL]]
```sql
CREATE TABLE IF NOT EXISTS javaeetodo.profil (profil_id int NOT NULL PRIMARY KEY GENERATED ALWAYS AS IDENTITY,
				 	profil_name character varying(30),
					profil_password character varying(30));

CREATE TABLE IF NOT EXISTS javaeetodo.tag (tag_id int NOT NULL PRIMARY KEY,
				 	tag_description character varying(30));
					
CREATE TABLE IF NOT EXISTS javaeetodo.todo(todo_id int NOT NULL PRIMARY KEY GENERATED ALWAYS AS IDENTITY,
				   todo_name character varying(30),
				   todo_description character varying(30),
				   creationdate character varying(10),
				   duedate character varying(10),
				   tag_id int REFERENCES javaeetodo.tag(tag_id),
				   profil_id int REFERENCES javaeetodo.profil(profil_id));
				   
CREATE SEQUENCE javaeetodo.sq_tag_tagid
    MINVALUE 0
    INCREMENT BY 1
    START WITH 0;		

CREATE OR REPLACE FUNCTION generate_key_value() RETURNS TRIGGER AS $$
    BEGIN
        IF NEW.tag_id IS NULL THEN
            SELECT NEXTVAL('javaeetodo.sq_tag_tagid') INTO NEW.tag_id;
        END IF;
        return NEW;
    END;
$$ LANGUAGE PLPGSQL;

CREATE TRIGGER trg_for_key BEFORE
INSERT ON javaeetodo.tag FOR EACH ROW EXECUTE PROCEDURE generate_key_value()
```


