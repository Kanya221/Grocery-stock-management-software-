# Grocery-stock-management-software-
Yogashree ra 204,rajashree ra208 and my self Kanya ra 221
def establishconnect():
    connectobject = db.connect("shopManagement.db")
    c = connectobject.cursor()
    sql = '''
    create table if not exists sell (
        date string,
        product string,
        price number,
        quantity number,
        total number
        )
    '''
    c.execute(sql)
    connectobject.commit()   
 
establishconnect()    
def connection2():
    connectobject2 = db.connect("shopManagement.db")
    c = connectobject2.cursor()
    sql = '''
    create table if not exists stock (
        date string,
        product string,
        price number,
        quantity number
        )
    '''
    c.execute(sql)
    connectobject2.commit()   
 
connection2()
