## Default Roles

<table>
    <tr>
        <th>Role</th>
        <th>Resources</th>
        <th>Create</th>
        <th>Read</th>
        <th>Update</th>
        <th>Destroy</th>
    </tr>
    <tr>
        <td>Owner</td>
        <td>
            <ul>
                <li>Organizations</li>
                <li>Account associations</li>
                <li>Role-bindings</li>
                <li>Organization invitations</li>
                <li>Custom roles</li>
                <li>Subscriptions</li>
            </ul>
        </td>
        <td>✅</td>
        <td>✅</td>
        <td>✅</td>
        <td>✅</td>
    </tr>
    <tr>
        <td>Editor</td>
        <td>
            <ul>
                <li>Images</li>
                <li>Clusters</li>
            </ul>
        </td>
        <td>✅</td>
        <td>✅</td>
        <td>❌</td>
        <td>✅</td>
    </tr>
    <tr>
        <td></td>
        <td>
            <ul>
                <li>Role-bindings</li>
                <li>Subscriptions</li>
            </ul>
        </td>
        <td>✅</td>
        <td>✅</td>
        <td>✅</td>
        <td>✅</td>
    </tr>
    <tr>
        <td></td>
        <td>
            <ul>
                <li>Policies</li>
                <li>Records</li>
                <li>Organizations</li>
                <li>Organization Invites</li>
                <li>Roles</li>
                <li>Account Associations</li>
            </ul>
        </td>
        <td>❌</td>
        <td>✅</td>
        <td>❌</td>
        <td>❌</td>
    </tr>
    <tr>
        <td>Viewer</td>
        <td>
            <ul>
                <li>Images</li>
                <li>Policies</li>
                <li>Records</li>
                <li>Organizations</li>
                <li>Organization Invites</li>
                <li>Clusters</li>
                <li>Roles</li>
                <li>Role Bindings</li>
                <li>Subscriptions</li>
                <li>Account Associations</li>
            </ul>
        </td>
        <td>❌</td>
        <td>✅</td>
        <td>❌</td>
        <td>❌</td>
    </tr>
</table>