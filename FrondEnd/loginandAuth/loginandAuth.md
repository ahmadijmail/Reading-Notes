# Login  and Auth 

## What is Role Based Access Control (RBAC)?

Role-based access control (RBAC) restricts network access based on a person's role within an organization and has become one of the main methods for advanced access control.

## An example of RBAC including all possible CRUD operations and correlating roles.

Through RBAC, you can control what end-users can do at both broad and granular levels. You can designate whether the user is an administrator, a specialist user, or an end-user, and align roles and access permissions with your employees’ positions in the organization. Permissions are allocated only with enough access as needed for employees to do their jobs.


Some of the designations in an RBAC tool can include:

Management role scope – it limits what objects the role group is allowed to manage.

Management role group – you can add and remove members.

Management role – these are the types of tasks that can be performed by a specific role group.

Management role assignment – this links a role to a role group.

## What are the Benefits of RBAC?

1. Reducing administrative work and IT support. 

2. Maximizing operational efficiency. 

3. Improving compliance.


**universal-cookie - Universal cookies for JavaScript**

**universal-cookie-express - Hook cookies get/set on Express for server-rendering**


## react-cookie

const [cookies, setCookie, removeCookie] = useCookies(['cookie-name']);

## react-cookies


*** 

```
import { Component } from 'react'
import cookie from 'react-cookies'
 
import LoginPanel from './LoginPanel'
import Dashboard from './Dashboard'
 
class MyApp extends Component {
  constructor () {
    super()
 
    this.onLogin = this.onLogin.bind(this)
    this.onLogout = this.onLogout.bind(this)
  }
 
  componentWillMount() {
    this.state =  { userId: cookie.load('userId') }
  }
 
  onLogin(userId) {
    this.setState({ userId })
    cookie.save('userId', userId, { path: '/' })
  }
 
  onLogout() {
    cookie.remove('userId', { path: '/' })
  }
 
  render() {
    const { userId } = this.state
 
    if (!userId) {
      return <LoginPanel onSuccess={this.onLogin} />
    }
 
    return <Dashboard userId={userId} />
  }
}
```
