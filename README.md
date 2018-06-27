# DFS
#adding edge
#counter for visited node
#dfs(int u)
{
        v[u]=true;
        vector<int>::iterator i;
        for(*i=edge[u].begin();*i!=edge[u].end();i++)
        {
                if(!v[*i])
                        dfs(edge[u][*i]);
        }
}
