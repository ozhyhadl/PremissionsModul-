# PremissionsModul-

class User {
  name: String
  role: [Role]?
  accessWrite: Bool
  accessRead: Bool
}

class Role {
    nameOfRole: String
    accessWrite: Bool
    accessRead: Bool
}

func setNewRole(nameOfRole, accessWrite, accessRead) -> Bool

func setRoleUser(user, role) -> Bool
func setAccessUser(user, accessWrite, accessRead) -> Bool

func isAccessUserWrite(user) -> Bool
func isAccessUserRead(user) -> Bool

Table User {
	name,
  role, //One-to-many 
	accessWrite,
	accessRead
}

Table Role {
	nameOfRole,
	accessWrite, 
	accessRead
}




