<!-- Esercizio di oggi: DB Auto
nome repo: db-first
Modellizzare la struttura di una tabella per memorizzare tutti i dati riguardanti delle auto usate messe in vendita da un concessionario.
Cerchiamo di immedesimarci nel contesto e di immaginare le colonne di una tabella auto e i relativi tipi di dato e attributi. -->

# USED AUTO

-- | TYPE | ATTRIBUTES
-- | -- | --
`id` | BIGINT | Primary Key - Unique - Auto_increment 
`brand` | VARCHAR(15) | Not Null 
`model` | VARCHAR(15) | Not Null 
`version` | VARCHAR(15) | Null 
`transmission` | TINYINT(1) | Not Null 
`registration_year` | DATE | Not Null 
`vehicle_identification_number` | CHAR(17) | Not Null - Unique 
`fuel_type` | TINYINT(1) | Not Null 
`euro_type` | TINYINT(1) | Null 
`seller_name` | DATE | Not Null 
`seller_lastname` | VARCHAR(15) | Not Null 
`purchase_date` | VARCHAR(15) | Not Null 
`km` | FLOAT(8,2) | Not Null 
`cost` | DECIMAL(8,2) | Not Null
`seats` | TINYINT(1) | Null 
`it_works` | TINYINT(1) | Not Null - Default(1) 
`defects` | TINYINT(1) | Null 
`administrative_detention` | TINYINT(1) | Not Null - Default(0)
`had_crash` | Not Null - Default(0) | Not Null - Default(0)
`optional` | TEXT | Not Null
