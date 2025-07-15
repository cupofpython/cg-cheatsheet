<table>
    <!-- Header -->
    <tr>
        <th>Action</th>
        <th>Example Command</th>
        <th>Tags</th>
        <th>Notes</th>
        <th>Use Cases</th>
    </tr>
    <!-- Start entry in the cheatsheet -->
    <tr>
        <td> <!-- Description -->
        Debug using entrypoint to dev variant
        </td>
        <td> <!-- Copy paste command -->
            <pre><code class="language-bash">docker run -it --entrypoint bash example-php-image
            </code></pre>
        </td>
        <td> <!-- Tags -->
            <ul>
                <li>N/A</li>
            </ul>
        </td>
        <td> <!-- Notes -->
            <ul>
                <li>Use the dev variant to have access to a shell and bash as the entrypoint to kickoff the shell on container start</li>
            </ul>
        </td>
    </tr>
    <!-- End entry in the cheatsheet -->
    <!-- Start entry in the cheatsheet -->
    <tr>
        <td> <!-- Description -->
        Debug with CDebug tool
        </td>
        <td> <!-- Copy paste command -->
            <pre><code class="language-bash">docker run --rm -d --user root --name nginx-container cgr.dev/chainguard/nginx:latest \
            && cdebug exec -it nginx-container
            </code></pre>
        </td>
        <td> <!-- Tags -->
            <ul>
                <li>N/A</li>
            </ul>
        </td>
        <td> <!-- Notes -->
            <ul>
                <li>This is under the assumption that CDebug is installed locally</li>
            </ul>
        </td>
    </tr>
    <!-- End entry in the cheatsheet -->
</table>