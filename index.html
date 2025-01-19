import streamlit as st
import asyncio
import asyncpg
import pandas as pd  # For better table visualization

async def fetch_data():
    conn = await asyncpg.connect(
        host='ep-morning-night-a1x54508.ap-southeast-1.aws.neon.tech',
        user='database_owner',
        password='BW0ah2JUCoeO',
        database='database',
        ssl='require'
    )
    # Use schema name in the query
    rows = await conn.fetch("SELECT * FROM bottle.bottle LIMIT 50")
    await conn.close()
    return rows

# Streamlit app
st.title("Neon Database with asyncpg")

# Fetch and display data
try:
    data = asyncio.run(fetch_data())
    if data:
        # Convert asyncpg.Record to a list of dictionaries
        formatted_data = [dict(row) for row in data]
        
        # Convert the list of dictionaries into a pandas DataFrame
        df = pd.DataFrame(formatted_data)

        # Display the data as a table in Streamlit
        st.dataframe(df)  # This will show the data in a table format with interactive capabilities
        
    else:
        st.write("No data found.")
except Exception as e:
    st.error(f"Error fetching data: {e}")
