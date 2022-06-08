## orm
- db().connect()
  - commit() close()
- Model
  - create()
    - save()
  - .execute()$
    - .select()
      - join where group_by order_by
    - .insert/replace()
  - get(:dsl)
    - get_or_none()
    - get_or_create(:dsl, defaults)
- class Table(Model):
  - col = *Field(...)
    - primary_key=False
    - unique=False
    - default=None
    - null=False 

     
