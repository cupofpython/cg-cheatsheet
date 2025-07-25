<table>
    <!-- Header -->
    <tr>
        <th>Action</th>
        <th>Example Command</th>
        <th>Flags</th>
        <th>Notes</th>
        <th>Use Cases </th>
    </tr>
    <!-- Start entry in the cheatsheet -->
    <tr>
        <td> <!-- Description -->
        Obtain registry token (publically available image)
        </td>
        <td> <!-- Copy paste command -->
            <pre><code class="language-bash">tok=$(curl "https://cgr.dev/token?scope=repository:chainguard/python:pull" | jq -r .token)
            </code></pre>
        </td>
        <td> <!-- Flags -->
            <ul>
                <li>N/A</li>
            </ul>
        </td>
        <td> <!-- Notes -->
            <ul>
                <li>Check for token by echoing, i.e. `echo $tok`</li>
            </ul>
        </td>
        <td> <!-- Use Cases -->
            <ul>
                <li>Used to call Chainguard API</li>
            </ul>
        </td>
    </tr>
    <!-- Start entry in the cheatsheet -->
    <tr>
        <td> <!-- Description -->
        Obtain registry token (private image)
        </td>
        <td> <!-- Copy paste command -->
            <pre><code class="language-bash">tok=$(curl -H "Authorization: Bearer \
            $(echo 'cgr.dev' | docker-credential-cgr get)" \
            -v "https://cgr.dev/token?scope=repository:chainguard/python:pull" \
            | jq -r .token)
            </code></pre>
        </td>
        <td> <!-- Flags -->
            <ul>
                <li>N/A</li>
            </ul>
        </td>
        <td> <!-- Notes -->
            <ul>
                <li>Check for token by echoing, i.e. `echo $tok`</li>
            </ul>
        </td>
        <td> <!-- Use Cases -->
            <ul>
                <li>Used to call Chainguard API</li>
            </ul>
        </td>
    </tr>
    <!-- End entry in the cheatsheet -->
        <!-- Start entry in the cheatsheet -->
    <tr>
        <td> <!-- Description -->
        Fetch tag history of an image
        </td>
        <td> <!-- Copy paste command -->
            <pre><code class="language-bash">curl -H "Authorization: Bearer $tok" \
            https://cgr.dev/v2/chainguard/python/_chainguard/history/latest | jq
            </code></pre>
        </td>
        <td> <!-- Flags -->
            <ul>
                <li>N/A</li>
            </ul>
        </td>
        <td> <!-- Notes -->
            <ul>
                <li>Obtaining registry token is required for this</li>
            </ul>
        </td>
        <td> <!-- Use Cases -->
            <ul>
                <li>Used to get image digests from previous builds, point to specific builds in Dockerfiles</li>
            </ul>
        </td>
    </tr>
    <!-- End entry in the cheatsheet -->
</table>